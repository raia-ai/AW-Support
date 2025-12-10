---
description: "EN-CONFIG-AW_iQuote_3"
---


---
## 4.7.1. Change processings

### Processing Add
Search the processing activity specified in the `SearchName` and insert a processing; this new processing is selected in the interface. It appears under the processing type specified in `ProcessingTyp`. This way, a macro can appear under edgework. If the `SearchName` is not specified, the first processing activity is found. With the activity, processings can be created from the workflow.

| Parameter | Description | Default |
| :--- | :--- | :--- |
| **Configurator** | Access to the Configurator service | Configurator |
| **ItemOut** | Initial item object of iQuote; the processing is inserted here | ItemOut |
| **NewProcessing** | The new processing data object | CartItemActionData Variable |
| **ProcessingType** | The processing type under which the processing appears | Enum ProcessingType |
| **ProductNo** | Product number of the processing to be inserted | |
| **SearchName** | Display name of the action validator to be searched for; if empty, the first one is found. | |

### Processing Update
Search the processing activity specified in the `SearchName` and change the processing; this changed processing is selected in the interface. It appears under the processing type specified in `ProcessingTyp`. This way, a macro can appear under edgework. If the `SearchName` is not specified, the first processing activity is found. With the activity, processings can be changed from the workflow. If the processing type changes, the parameters are lost.

| Parameter | Description | Default |
| :--- | :--- | :--- |
| **Configurator** | Access to the Configurator service | Configurator |
| **ItemOut** | Initial item object of iQuote; the processing is inserted here | ItemOut |
| **NewProcessing** | The changed processing data object | CartItemActionData Variable |
| **ProcessingType** | The processing type under which the processing appears | Enum ProcessingType |
| **ProductNo** | Product number of the changed processing | |
| **SearchName** | Display name of the action validator to be searched for; if empty, the first one is found. | |

### Processing Delete
Search the processing activity specified in the `SearchName` and delete the transferred processing; the first processing is then selected. With the activity, processings can be deleted from the workflow.

| Parameter | Description | Default |
| :--- | :--- | :--- |
| **Configurator** | Access to the Configurator service | Configurator |
| **ItemOut** | Initial item object of iQuote; the processing is inserted here | ItemOut |
| **Processing** | Processing object that is to be deleted. Can be searched for with "Processing Find." | CartItemActionData Variable |
| **Removed** | True if the processing was deleted; otherwise false | |
| **SearchName** | Display name of the action validator to be searched for; if empty, the first one is found. | |

### Processing Find
Search the processing activity specified in the `SearchName` and in that, search for the processing with the transferred product number or by processing type. The processing is returned or an empty object `<nothing>`. With the activity, processings can be found from the workflow, which are then deleted or changed.

| Parameter | Description | Default |
| :--- | :--- | :--- |
| **Configurator** | Access to the Configurator service | Configurator |
| **ItemOut** | Initial item object of iQuote; the processing is inserted here | ItemOut |
| **Processing** | Return of the found processing data object. If nothing was found, the return is `<nothing>` null. | CartItemActionData Variable |
| **ProcessingType** | The processing type that should be searched for. Only the processing type or product number can be specified. | Enum ProcessingType |
| **ProductNo** | The product number that should be searched for. Only the processing type or product number can be specified. | |
| **SearchName** | Display name of the action validator to be searched for; if empty, the first one is found. | |

## 4.8. Multilingual Workflow
iQuote is multilingual via the URL; this means that all fixed texts are output in the appropriate language. In order to activate this, the language abbreviation (e.g. `../en`, `../de`) must be attached.

However, the workflow is created customer-specifically and thus here there is also the need to enable this easily. The duplication of the workflow for each language is surely not the correct solution. The maintenance of the workflows would suffer for this.

The multilingual texts are managed in the table `Core_CustomTexts`, currently there is no management program for this. It would make sense to create an Excel table. This could be translated and then Insert Statements created with the help of the Excel table.

```sql
INSERT INTO [Core_CustomTexts]
([Guid], [VersionId], [LockingToken], [Code], [LanguageCode], [Text], [Comment]) VALUES
(newid(),1,'00000000-0000-0000-0000-000000000000', <Code nvarchar(255)>, <LanguageCode nvarchar(5)>, <Text nvarchar(max)>, <Text nvarchar(max)>)
```

These must then be executed in the SQL Server Management Studio. The subsequent editing can also be done there.

The language codes ('LanguageCode' column) correspond to the `Core_Languages` table.

```sql
SELECT TOP (1000) [Guid]
      ,[VersionId]
      ,[LockingToken]
      ,[Code]
      ,[Description]
FROM [Core_Languages]
```

In order to use these texts in the workflow, there are 2 possibilities:

1.  **Via function `Configurator.GetCustomText(code, languageCode)`**
    Definition of a global variable for assignment of `Cart.CurrentItem.Culture`. A `LanguageCode` variable is created and assigned the value `Cart.CurrentItem.Culture`.

2.  **Via language code sequence „@@<code>@@"**
    To simplify this, in an activity (not in an expression) without function call, there can be a text fetching; for this, the message code must have a "@@" in front of it and be attached. The function is then expanded internally and the `Configurator.CustomMessage("Test", )` function is called. For example, a property can be set to `"@@CategoryProduct@@"`.

## 4.9. Dynamic values for the workflow
The workflow can now save dynamic values in the `DynamicValues` properties of the `Cart` and `CartItem`. These values are saved in the database and always re-presented to the workflow in its `ItemIn` property. The workflow must ensure that they are transferred to the `ItemOut`.

The Activities `DynamicValuesGet()` delivers a value identified by a string. `DynamicValuesAdd()` stores it again. If the value is already there, it is overwritten.

This way, the workflow can now store any data in the workflow that it needs for calculations or comparisons.

### DynamicValuesGet
Search in the dynamic values for a specified key. If it is present, the value is returned; otherwise an empty string.

| Parameter | Description | Default |
| :--- | :--- | :--- |
| **DynamicValues** | Collection of the dynamic values | itemIn.DynamicValues |
| **Key** | Key string for the value | |
| **Value** | Delivers the value for the key transferred; if it is not there, then the value is empty | |

### DynamicValuesAdd
Inserts a dynamic value with a specified key. If it is present, the value is overwritten.

| Parameter | Description | Default |
| :--- | :--- | :--- |
| **DynamicValues** | Collection of the dynamic values | itemIn.DynamicValues |
| **Key** | Key string for the value | |
| **Value** | Delivers the value for the key transferred; if it is not there, then the value is empty | |

## 4.10. Access to the iQuote data structures
The workflow uses the internal data structures of iQuote and transforms this into new widget data that appears on the interface. An iQuote without workflow is just an empty shell. In this process we intervene with ready-made widgets, but it may also be necessary to access this data via Visual Basic (the programming language of the workflow). This article describes the necessary steps to implement this.

First you have to define where to add your code. Checkin-, checkout-, configuration- or mapping workflow. For this example I decide to use the configuration workflow and want to access the checkin data "Customer item" or "Commission". The argument given to this workflow is the `cart`.

This `cart` has 3 properties for the different workflows: `Cart.Checkin`, `Cart.Checkout` and `Cart.CurrentItem`. I need access to `Cart.Checkin`. `Cart.checkin` has a collection of `ItemActions`, which is a collection of `CartItemActionData`. All widget data objects are children of this collection. To get the widget data for the order, you need the data object of this widget. The default display name is "DeliveryText Reference".

First I create a variable locally in a sub-workflow of the widget's data type, for example `myCommonItemRemark` of type `CommonItemRemark`.

Then the selected `ItemRemark` object can be assigned to your "myCommonItemRemark" object variable with this Visual Basic Linq statement:

```vbnet
TryCast(cart.CheckIn.ItemActions.FirstOrDefault(Function(c) c.DisplayName = "DeliveryText Reference").SelectedData, CommonItemRemark)
```

For more information about Linq, please google "Visual Basic Linq 101" on the web for help. You can now access the customer position with `myCommonItemRemark.CustomerItem`.

The ILSpy software can be used to find out the shape properties.

## 5. Master Data Consolidation
Before the introduction of iQuote, it must be checked whether the current master data for order entry is designed for the use of iQuote.

Here it must be considered that the end customer who enters a glass via iQuote does not have the knowledge of a trained employee of the customer and thus also does not know the customer's internal structures and work instructions and also should not know these.

This means that all special tasks that a person entering an order must perform to enter a product must be done by iQuote automatically; if not, products will be entered incorrectly via iQuote. If this is not possible for a product, it may not be enabled for iQuote.

Examples that an end customer cannot perform in iQuote:
- There is a process that in case of a particularity, the person entering the order creates a text (e.g. inserts a correct text or simply overwrites the product designation of a processing), this text is printed everywhere in production and heeded.
- Under particular circumstances, a dummy article is attached to the item or order that influences the price.

Most of these things should be resolved with appropriately-maintained master data or through use of the correct functions. This can mean a consolidation of the master data, which can be associated with a lot of effort on the customer's part, The result will also be, in addition to the possible use of iQuote, easier entry.

In order to find out if something must be adjusted, the customer should play through the entry of the products that are enabled in iQuote and check whether there are any particularities that a layperson cannot know and thus could make an error.

In this document, individual examples are listed that have occurred at customers.

### 5.1. Precise product designations
Using the product designation, the end customer should understand what he is selecting. If, for example, a processing includes cryptic abbreviations that everybody at the company understands, it is not necessarily the case that the end customer understands these too.

### 5.2. Hole drillings for different diameters
For a hole drilling processing, you can define in the master data in which diameter range the processing may fall. This must be maintained if you would like to work with the following processings, for example:
- Hole drilling <= 20mm
- Hole drilling > 20mm

If this restriction is not maintained, then you can use the processing `<= 20 mm` for a 30 mm hole, which may mean a cheaper price. The person recording the order can receive a work instruction in order to select the correct processing, the end customer cannot.
Through the restriction it is ensured that the selected diameter fits the processing. However, it is much more elegant to have just one processing for all diameters. There is no (more) reason to have several. The price calculation can orient itself according to the diameter entered, it does not have to orient itself using the processing article.

### 5.3. Entering the correct edge processing
For the entry of edge processing, there are several scenarios that require the deeper knowledge of the person entering the order. The person entering the order knows which edge processing he must apply how, but the end customer does not know this.
- On a sheet, several edge processing are entered for the same edge quality, e.g. polish straight edge, polish round edge, polish special edge. You do this, e.g. due to the price calculation, rounding is more expensive than a straight edge.
- A shape where all edges should be polished. The straight edges should be ground on a normal grinding machine (which may only be able to process straight edges), the arches on a CNC (which can grind everything but is slower and more expensive).

At the latest starting with AWB 5.5, there is no more reason to use several edge processings for the same edge quality. See on this the A+W Business configuration documentation, chapter on Shape edge additions.

If this is introduced, it simplifies normal entry and thus has a big added value for the customer regardless of iQuote.

### 5.4. Use of color variants
If you enter a surface processing, e.g. for a finish, you should work for the selection of colors with appropriate color variants and not just write the color code (e.g. RAL) manually next to the product designation of the processing. Since you do not want to enter variants for all possible color codes since there would be too many, you can enter a variant for special colors in addition to the common ones For this variant it is possible to write the appropriate color code in a field (that appears when this variant is selected). This field is transferred to production and should be available in iQuote as soon as case #350715 has been implemented.

In addition, for the color variants in the master data, you can also store a color code for the display, which is then depicted in iQuote in this color.

### 5.5. TG always with complete BOM
An edge processing must always be present in the BOM of TG, at least a seaming. If this is missing in the product's BOM, then during order entry an edge processing must always be applied, even in iQuote. If this is forgotten, a TG without edge processing is created.

If there is already a seaming in the TG's master data, then it is also not possible to enter an incorrect product. If the customer would like a higher-quality edge processing, this can be entered easily; iQuote then reduces the lower-value processing (seaming).

## 6. CSS Customizing
If the CSS is changed for a customer, then you must pay attention that it must be reworked with each new version. Thus, permanent work and costs are required.

### 6.1. General information and basic principles
There is a setting that is definitely helpful when testing design adjustments: it can be specified that with each refresh of the website (that is, when you press F5 in the browser) that the .less files are recompiled. Thus, changes will be effective immediately. However, this is at the expense of the performance, so it is not intended for productive operation.

For this, in the file `C:\Sandpiper1\WebWeb\web.config` in the line `<compilation targetFramework="4.5">` the entry `debug="true"` must be added.

```xml
<system.web>
    <httpRuntime targetFramework="4.5" maxRequestlength="1048576" />
    <compilation targetFramework="4.5" debug="true">
        <assemblies>
            <add assembly="System.Web.Abstractions, Version=4.0.0.0, Cultu..."/>
            ...
        </assemblies>
    </compilation>
</system.web>
```

For the conversion to live operation, it is not necessary to restore the original file. It is sufficient to change the value from `debug="true"` to `debug="false"`.

Generally, the custom theme should always be used for design adjustments. The theme can be specified in the infrastructure configuration as follows:
In the Infrastructure settings, under Website Settings, set the `Theme` to `Custom`.

Alternatively, it is possible to access the custom theme regardless of the preconfigured theme. For this, the addition `?theme=custom` must be made to the iQuote URL. However, the prerequisite is that in the infrastructure configuration, the value of the entry `Theme is Mandatory` is on `Off`.

This way, you can also access all other themes:
- Uniform
- Black
- Default
- Metro
- Metroblack
- Custom

**Note:** The browser notes the last theme loaded. If you want to change from the custom theme back to the original theme (Uniform), it is not sufficient to leave off the parameter in the iQuote URL again. Instead, you have to specify the standard theme as URL parameter one time. Alternatively, you can delete the browser data.

Otherwise, it is frequently helpful to reset the IIS so that changes become effective. For example, this is the case if you want to change icons (bootstrap glyphicons). That's to say: if you wonder why a change is not effective immediately, it's best to restart the IIS. The A+W iQuote services play no role here.

Colors can always be specified in the CSS in different ways. You can make wild combinations. Here's an example:
- Hex color: `#0070c0`
- Red-green-blue: `rgb(255,99,71)`
- Red-green-blue-Alpha: `rgba(255,0,0,0.5)`
- Name of the color (only particular ones): `darkblue` -> You can also write `transparent`!

### 6.2. How custom theme works
The custom theme is found under the following path:
`C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\Custom`

Critical here are the two files `kendo.custom.less` and `awsoa-responsive.custom.less`.

The file `kendo.custom.less` forms the design basis. On the website of the Kendo provider, there is a configurator where you can build standard themes yourself. The focus is mostly on text colors, colors of titles, background colors, etc. You can download a finished theme and transfer its content to the actual file.
(See: Custom Theme Builder | Kendo UI for jQuery on telerik.com)

**Note:** Here you specify basic settings, however the effects are not immediately visible. This is because the file is sometimes overridden.

The file `awsoa-responsive.custom.less` imports the file `kendo.custom.less`. Here, individual settings can be overridden. It's easy to trace this with the entry `@image-folder`, which is present in both files. For the file `kendo.custom.less`, the value is "Uniform" and for the file `awsoa-responsive.custom.less`, the value is "Default".

Intended are always the folders with the same name in the path `C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\kendo`. That the entry comes from the `awsoa-responsive.custom.less` file is easy to see using the example of the load icon in iQuote. The icon that is in the `Default` folder is displayed.

The `awsoa-responsive.custom.less` file also calls a particular template file. By default, this is `C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\awsoa\awsoa-theme-template-responsive.less`. This file is commented and here you can test various changes in the browser and then build them permanently into the template file after the fact.

### 6.3. Overriding rules and own CSS rules
This point is probably one of the most important ones.

The later a command comes in the `.less` file, the higher it seems to be prioritized. It is possible to build your own CSS rules into `.less` files, which you can design directly in the browser. At least with the Chrome browser, this works very well:

For this, you have to right-click on the element you'd like to examine and then select `Inspect` from the context menu.

Then the selected element is highlighted in color on the left side and on the right side you can see the associated CSS rules. The rules that are crossed out do not apply because they are overridden, for example. The active rules can be edited directly and you can examine the result live in the browser.

An example of where the background color was overridden by precisely this button is at the end of the included `awsoa-responsive.custom.less` file.

This way, it is possible to construct all of your own rules for any element and to execute them. The full spectrum of CSS rules is available. These include:
- Changing the font size and type
- Turning and stretching elements
- Editing button sizes
- Configuring backgrounds/fillings with particular color gradients
- Adding your own new elements (e.g. displaying a new image)

### 6.4. Background color on the main menu
**File:**
`C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\Custom\awsoa-responsive.custom.less`

**Value:**
`@carusell-foo1-background`

### 6.5. Colors of iQuote navigation bar
**File:**
`C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\Custom\awsoa-responsive.custom.less`

**Values:**
- Background color of the whole bar: `@navbar-background-color`
- Text color in general: `@navbar-text-color`
- Color of the rectangles around the fields: `@navbar-border-color`
- Fill color of the field you have just selected: `@navbar-active-background-color`
- Fill color of the fields if you point to them with the cursor: `@navbar-text-hover-color`
- Text color of the fields if you point to them with the cursor: `@navbar-text-hover-color`

### 6.6. Colors of configurator navigation bar
**File:**
`C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\Custom\awsoa-responsive.custom.less`

**Values:**
- Text color: `@breadcrumb-text-color`
- Color of the surrounding rectangles: `@breadcrumb-border-color`
- Fill color of the category you have just selected: `@breadcrumb-selected-color`
- Fill color of the categories not selected: `@breadcrumb-completed-color`

### 6.7. Change load icon
**File:**
`C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\Custom\awsoa-responsive.custom.less`

**Value:**
`@image-folder: "default";`

**To Do:**
In the directory `C:\Program Files (x86)\A+W\Sandpiper1\WebWeb\Content\kendo`, create a new folder. Then, in the file `awsoa-responsive.custom.less`, set the value of `@image-folder` to the name of the new folder.
Exchange the file `loading-image.gif` in the new folder.
Alternatively, you can change it directly in the `Default` folder.

## 7. Login page configuration
The prerequisite for the configuration is the installation of the A+W iQuote login page as described in the A+W iQuote installation instructions.

The concept behind the login page is that it is a page before A+W iQuote. On it, user logins are managed; users can register themselves. The user is assigned an iQuote instance.

Registration of the iQuote is done with a one-time token. The iQuote trusts the login page; a user who has authenticated himself on the login page is also authenticated in iQuote. The login page and the iQuote have a trust relationship that is secured with the private key. Only if it is the same in both systems do the systems trust each other. A user's login data cannot be used to log in into the stand-alone iQuote. The customer employee login data still works on the stand-alone iQuote, however; it must be deleted.

### 7.1. Initial login as administrator
First, there must be a login with the user `admin@a-w.com` and the password: `Adm1n!`. Then a new Admin user should be created and the existing Admin user deleted. The new user becomes an Admin based on their role. There can be several and if the access to the mail address exists, the password can also be changed.

> **Attention:** if there is no more Admin access, the login page can no longer be administered. Then the database must be deleted or the admin role assigned to a user via SQL.

### 7.2. Pages
For each site, the URL of the iQuote and if necessary the token URL must be entered. These can differ if there are restrictions between internal and external access. Normally they are the same.

The access from the login page to the iQuote is authorized via a token; for this, however, the comparison of a private key is required. This private key must be stored here (in the Login Page settings) and in the A+W Business company master data.

Essentially, a default private key is always returned, even if none is entered in A+W Business. This is a safety feature and prevents uncontrolled access to the system.

> **CAUTION:** a private key must be compared between the login page and A+W Business; otherwise no connection can be established. Leaving this blank is not an option.

In addition to the private key, the IPv4 or IPv6 of the login page server must be entered here. Only queries from this computer are permitted.

> **CAUTION:** If permitted IPs are entered, the ipv6 must absolutely be stored ( ":::1" is the local host). If no IP is entered, then there is also no check; this is a safety feature and should be used if possible.

The default customer initially serves to map a newly created user to the various customers. This way, a private customer can also log in and order products. If this feature should not be possible, this field must be left empty.

A+W iQuote is a B2B configurator; an entry of the default customer number opens the configurator as B2C. Here, however, there are various requirements for the contract conclusion, payment methods that can conflict with the country's laws. This must first be clarified.

If the login page has been activated, then the entry of the iQuote password in the customer employee management is no longer possible. The business case can then be stored in the customer management.

### 7.3. User
If a user is created by the administrator, the user receives a mail with the prompt to assign a password. This mail has a link with a token that is mandatory for the registration.

The customer number defines with which customer the user is logging into A+W Business. If this is 0, then the default customer of the corresponding page is used. If this is also 0, the user can only log in on the login page, but not change to iQuote.

> **CAUTION:** The mail to the user contains a link with the address (URL) of the login page. This link address is controlled via the browser's address bar. If the login page is called from an internal address, the mail contains an internal address link. With it, it is not possible for the user to set his password, however. Attention must always be paid that the user registration is done from the public URL. It's best if the computer in the DMZ doesn't have a local address (DNS) and everyone must always go via the external URL!!!

### 7.4. Links
Via `Administration->Links`, links to videos (YouTube) and PDF documents can be entered. They then appear on the login page.

The URL and symbol URL must be specified for PDF links with a relative path, e.g., "Content/...". There is no access to files from other domains, except for video. The first entry is displayed automatically.

### 7.5. Settings
Via the self-registration, the possibility can be switched off that a customer can register themselves. If this is deactivated, then only the Administrator can register customers and send them an invitation mail. In connection with the default customer number, the self-registration creates a B2C configurator. Here, however, there are various requirements for the contract conclusion, payment methods that can conflict with the country's laws. This must first be clarified.

Access to the mail server must be configured; this can be checked with the Test Mail button. The registered Administrator then receives a mail. If an employee should be informed about all documents, this person can be entered as BCC (blind copy) or as CC.

### 7.6. User self-registration and password reset
Via the link on the login dialog, a user can register themselves and also reset their password. The prompt for this comes via mail.

### 7.7. Customizing the login page

#### 7.7.1. View layout for customizing
The login page is completely customizable; this affects the CSS part (see Chapter 6) as well as the HTML part.

The login page always starts with the custom theme if the following files are stored under `Content\custom`:
- `~/Content/Custom/custom.css`
- `~/Content/Custom/kendo.custom.less`
- `~/Content/Custom/awsoa-responsive.custom.less`

The `Custom.css` can contain CSS that does not have a direct relationship with Kendo. It can also be empty, but for recognition, it must be in the folder. These files can also be obtained from the `Custom` directory of the iQuote.

For this, custom cshtml pages (ASP.NET Razor Syntax) must be created that are called exactly the same as the originals.

The view structure is as follows:
- Views
  - Account
  - Custom
    - Home
      - `PartialMain.cshtml`
  - Home
    - EditorTemplates
    - `Index.AWB.cshtml`
    - `Index.cshtml`
    - `PartialAbout.cshtml`
    - ...
    - `PartialMain.cshtml`
    - ...
  - Manage
  - Shared

The customized page of the main view of the login page is in the `Views->Custom->Home` directory. The menu is implemented in the `PartialNavbar.cshtml`; here, for example, extensions to the menu can be entered.

If a department-specific view is present, then the custom view must have the same name, e.g. `Index.AWB.cshtml`.

#### 7.7.2. Custom header and footer
If on the main page only an individual header and footer should be inserted, this can be done easily with the views:
- `~/Views/Custom/Home/CustomHeader.cshtml`
- `~/Views/Custom/Home/CustomFooter.cshtml`

The advantage of this solution is that the "PartialMain.cshtml" view must not be adjusted and thus the login page can still be updated.
To find these files, the login page must be in the custom theme; on this, see 7.7.1.

#### 7.7.3. Adding a view on the menu
If on the menu of the login page a new view should be incorporated, then first a copy of the `PartialNavbar.cshtml` must be created in the `Custom->Home` folder.

The menu can then be extended at any point there. For example, to add an "Addon" item:

```html
<li id="navbar-item-addon"><a href='javascript: vmMain.loadCustom("PartialAbout")'>Addon</a></li>
```

The JavaScript function `loadCustom()` must only be given the name of the view to be displayed. The extended menu then looks as follows, with an "Addon" button next to "About".

#### 7.7.4. Access to customer texts
Access to the texts from the table `Core_CustomTexts` (see also Chapter 4.8) is via the following command in a CSHTML view. The character `@` introduces C# code.

```csharp
@HttpContext.Current.GetCustomMessageString(“MYTEXT")
```
This is especially important for the creation of individual views on the login page in order to guarantee multilingual functionality.

#### 7.7.5. Adjustment of the customer mails
For registration and password change, the login page sends mails to the user; these are in a multilingual default. Of course customers need to adjust these to suit their corporate identity. For this, the login page offers the opportunity to define these individual texts differently in the customer texts. These texts are HTML-capable. To create them with SQL, see Chapter 4.8.

The following codes are reserved for the mail subject and body and must be entered into the customer texts:
- `WebLoginSendMailRegisterSubject`
- `WebLoginSendMailRegisterBody`
- `WebLoginSendMailResetPasswordSubject`
- `WebLoginSendMailResetPasswordBody`

Here are examples for inserting customer texts:
```sql
INSERT INTO [Core_CustomTexts]
([Guid], [VersionId], [LockingToken], [Code], [LanguageCode], [Text], [Description])
VALUES (newid(), 1, '00000000-0000-0000-0000-000000000000',
N'WebLoginSendMailRegisterSubject', 'de-DE', N'A+W Registrierung', N'');

INSERT INTO [Core_CustomTexts]
([Guid], [VersionId], [LockingToken], [Code], [LanguageCode], [Text], [Description])
VALUES (newid(), 1, '00000000-0000-0000-0000-000000000000',
N'WebLoginSendMailRegisterBody', 'de-DE', N'<html><p>Sie haben sich registriert in unserem Konfigurator</p><p>Bitte aktivieren Sie ihr Konto und vergeben sie ein Passwort. Klicken bitte <a href="{0}">hier</a></p></html>', N'');

INSERT INTO [Core_CustomTexts]
([Guid], [VersionId], [LockingToken], [Code], [LanguageCode], [Text], [Description])
VALUES (newid(), 1, '00000000-0000-0000-0000-000000000000',
N'WebLoginSendMailResetPasswordSubject', 'de-DE', N'A+W Passwort Zurücksetzen', N'');

INSERT INTO [Core_CustomTexts]
([Guid], [VersionId], [LockingToken], [Code], [LanguageCode], [Text], [Description])
VALUES (newid(), 1, '00000000-0000-0000-0000-000000000000',
N'WebLoginSendMailResetPasswordBody', 'de-DE', N'<html><p>Sie haben ihr Passwort vergessen.</p><p>Bitte vergeben Sie ein Neues. Klicken bitte <a href="{0}">hier</a></p></html>', N'');
```

For the mail body texts, a placeholder for the link address with `{0}` must be provided, otherwise the mail will not contain a link.

## 8. Login page Okta configuration
The prerequisite for the configuration is the installation of the "A+W iQuote login page Okta" as described in the A+W iQuote installation instructions.

The concept behind the login page is a page before A+W iQuote. User logins are managed by an Okta Tenant. The user is assigned an iQuote instance. Registration of the iQuote is done with a one-time token. The iQuote trusts the login page. The login page and the iQuote have a trust relationship secured with a private key. The stand-alone iQuote login page is deactivated and thus cannot be reached. A simultaneous operation of both login systems is not possible.

### 8.1. Okta platform configuration
Essentially, configuration of the Okta platform can be done in two ways. First manually (not recommended) or through Terraform. Using this tool, it is possible to use a superior configuration language to bring a cloud or the local infrastructure into the desired state for execution. First, download the command line tool [Terraform by HashiCorp](https://www.terraform.io/). The tool must be placed together with the configuration file (`C:\SANDPIPER1\WebLoginOkta\okta.tf`) in a secure place (e.g., `C:\Okta`). This is necessary since after executing the tool, a state screen for the Okta configuration is created. This may not be lost!

For the initial configuration, a command line is started. In the command line, you navigate to the folder `C:\Okta` with the following command:
```
cd C:\Okta
```
First a token must be generated that allows Terraform to make changes to the Okta tenant. A new token is created for this in the Okta admin panel on the left menu under "Security->API" -> "Tokens" -> "Create token".

This token must be entered in the `okta.tf` file under the `api_token` element. For the `org_name` and `base_url`, see the Okta admin panel.

```
provider "okta" {
  org_name = "dev-97365395"
  base_url = "okta.com"
  api_token = "<TOKEN>"
}
```

In addition, the URL that points to the "A+W Web Login Okta" must be entered with `https://` as follows:
```
variable "WebLoginUrl" {
  type = string
  default = "<WEB_LOGIN_HTTPS_URL>"
}
```

After these changes have been made, Okta can be configured with Terraform. This is done in the same folder via the command line using the following commands:
```
terraform init
terraform plan
terraform apply
```

#### 8.1.1. Creating a group and assigning a client
A client is represented in Okta by a group. For this, first you must create a new group and then assign it to the "iQuote" application. Ideally, the group has the same name as the client. On the menu on the left side, select "Directory" and then the "Group" menu element.

Then you open the group and assign the "iQuote" application on the "Applications" tab. For this, the URL of the iQuote instance must be entered. Important here is that the iQuote is hosted via a SSL encryption (HTTPS).

#### 8.1.2. Creating a user and connecting with an ERP customer
On the Okta admin panel, select the "Directory->People" element with the left menu and click "Add person".

Here, the screen must be filled out with the user data. Important is that for the "Groups" element, the group is entered that corresponds to the desired client.

To complete the user configuration, you must create an assignment to an ERP customer. To do this, select the user just created. After the user has been selected, click on the pen in the "iQuote" area on the "Applications" tab. You can enter the `ERPCustomerID` on the screen that opens. Here, either the default customer or a specific one can be selected.

#### 8.1.3. The default customer
The default customer initially serves to map a newly created user to the various customers. This way, a private customer can also log in and order products. If this feature should not be possible, this field must be left empty.

A+W iQuote is a B2B configurator; an entry of the default customer number opens the configurator as B2C. Here, however, there are various requirements for the contract conclusion, payment methods that can conflict with the country's laws. This must first be clarified.

If the login page has been activated, then the entry of the iQuote password in the customer employee management is no longer possible. The business case can then be stored in the customer management.

### 8.2. Configuration of "A+W iQuote Okta login page"
To switch the new login page live, the "A+W iQuote Okta Login Page" of the Okta tenant must be made known. This is done with the configuration file `C:\SANDPIPER1\WebLoginOkta\appsettings.json`. The "Okta" rubric must be configured in this file.

```json
"Okta": {
  "OktaDomain": "https://<OKTA_TENENT_HERE>.okta.com",
  "ClientId": "<CLIENT_ID_HERE>",
  "ClientSecret": "<SECRET_HERE>",
  "AuthorizationServerId": "default",
  "UseRedirectModel": "true"
},
```

For "OktaDomain", see the Okta admin panel. Important is that `https://` is placed in front of the Okta domain.

For the "ClientId" and "ClientSecret", use the left menu to navigate to the "Application" "iQuote" in Okta. Here, the values can be viewed and entered.

In the "Clients" area of `appsettings.json`, the private key for the client in question must be stored. For the clientID, see the A+W Infrastructure Web.
```json
"Clients": {
  "default": {
    "PrivateKey": "82FFECF2-5743-4E10-9D59-D0AD52298876"
  },
  "1": {
    "PrivateKey": "82FFECF2-5743-4E10-9D59-D0AD52298876"
  },
  "2": {
    "PrivateKey": "82FFECF2-5743-4E10-9D59-D0AD52298876"
  }
}
```
This private key must be stored here and in the A+W Business company master data.

> **CAUTION:** a private key must be compared between the login page and A+W Business; otherwise no connection can be established. Leaving this blank is not an option.

> **CAUTION:** If permitted IPs are entered, the ipv6 must absolutely be stored ( `":::1"` is the local host). If no IP is entered, then there is also no check; this is a safety feature and should be used if possible.

To apply the configuration, the "Web.Login.Okta" page in the IIS manager must be restarted.

### 8.3. Preparation of iQuote for the Okta login
In the Infrastructure Web, the logout detour to the login page must be configured.
- **Log out redirect active:** ON
- **Log out redirect URL:** `https://localhost:44314/Account/SignOut`

Under the element "Log out redirect URL", the web address of the login page must be entered. Important here is that the extension of the URL includes "/Account/SignOut".

**NOTE:** The "Okta" rubric point can be ignored initially since it does not contain any function.
To apply the configuration, the "Web.Web" page in the IIS manager must be restarted.

### 8.4. Customization
As "deployment model", "A+W iQuote Login Okta" relies on the Okta redirect model. See [Okta's documentation](https://developer.okta.com/docs/guides/redirect-vs-embedded/) to learn more about this. This means that the entire customization happens via Okta itself; see also [Style the sign-in page | Okta Developer](https://developer.okta.com/docs/guides/style-the-sign-in-page/main/).
