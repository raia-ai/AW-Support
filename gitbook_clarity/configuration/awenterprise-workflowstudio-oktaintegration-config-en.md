---
description: "EN-CONFIG-AW_Enterprise_iQuote_3"
---


---
## Projects Workflow Activity

> **UI Screenshot: Checkin Objects**
> A screen titled "Objects" shows a list of objects that can be added to an order. The objects are "QS Objekt2" and "Flughafen Eschbach".

The "Projects" workflow activity is in the "IQuote InOut" area of the Workflow Studio and must be used in the Checkin workflow.

> **UI Screenshot: Workflow Studio**
> The Workflow Studio interface shows the "iQuote InOut" toolbox on the left. A red arrow points from the "Projects" activity in the toolbox to a position in the "iQuote Check In AUW60" workflow diagram. The properties for the selected activity are shown on the right, with fields like `Category`, `ContentPath`, `CustomerNumber`, and `ObjectNumber`. The `ObjectNumber` property is set to `Cart.Header.ObjectNo`.

The activity has to be added to the Checkin workflow. The project number is stored in the `Card.Header.ObjectNo`. In the configuration workflow, it is therefore possible to access the project no. again. The parameterization is documented under 4.4 in the EN-CONFIG-A+W iQuote.

The Checkin workflow created must still be activated for the A+W iQuote. You can do this directly in the Workflow Studio (Configuration > Workflow management) or in the Infrastructure.Web dialog Workflow.

> **UI Screenshot: Workflow Management**
> A table displays different workflow extension points and their associated workflow files, types, and clients.

If a customer has not been assigned a project in A+W Enterprise, the selection of projects does not appear. If a customer has selected a project in A+W iQuote, then he cannot change the project he has selected in the current configuration after the fact; instead, he must discard this configuration.

## 15.4. Stock inventory display of an article from several clients

With the ticket [AW-116098], a possibility was developed to display the stock inventory of an article with respect to several clients.

Decisive for proper data in the front end is the back end stored procedure `"cu_lamgetcurrentstock."` Stored in the back end under `/develop/sql_scripts/cust/la` is a base variant of the Stored Procedure.

Without this stored procedure, no data is displayed in the front end.

**CAUTION:** Currently, no variant or color number from the A+W iQuote and the stored procedure is transmitted.

Similarly, it must be communicated to the front end that you would like to display the new switch. You do this in the Workflow Studio. There, you open the main workflow of the A+W iQuote that should be changed.

Example:

> **UI Screenshot: Open Workflow Dialog**
> A dialog box titled "Open Workflow" lists various system and predefined workflows, such as "iQuote Check Out Business" and "iQuote Enterprise".

There, you can enable the new stock inventory switch for each product type and product group. For this, you must click the ValidatorProducts of the desired product branch and set the switch `"OptionShowStockOnSites"` to `"True."`

The default is `"False."`

> **UI Screenshot: Workflow and Properties**
> A workflow diagram shows a path from `ValidatorProductGroups` to `ValidatorProductTypes` to `ValidatorProducts`. The properties pane for `ValidatorProducts` is displayed, with the `OptionShowStockOnSites` property highlighted and set to `True`.

After that, the Web Configurator in the Service Locator Administrator must be restarted so that the workflow can be reloaded.

> **UI Screenshot: Product Selection with Stock Information**
> The A+W iQuote interface shows product categories and products. A "Lager" (Stock) button is visible. Clicking it opens a dialog showing stock levels.

If it is not possible to determine any data, then an empty dialog window opens.

This logic depends on the stored procedure mentioned above.

> **UI Screenshot: "Auf Lager" (In Stock) Dialog**
> A small dialog shows the stock quantity for a product at a specific site ("Mandant"): Pohlheim (Vers 14.0) DE, Menge: 1.

## 15.5. Item reference text in shopping cart

With the development for [AW-74479], it is now possible to display the item reference texts in the shopping cart.

> **UI Screenshot: Item References in Configuration**
> The configuration screen for a product shows a "References" section where a user can enter reference text, for example, "House 1".

> **UI Screenshot: Item References in Shopping Cart**
> The shopping cart view shows an item "Float 4mm" with its details. The reference text "Float with polished edges/House 1" is highlighted, demonstrating that it is now visible in the cart.

To activate the logic, in A+W Infrastructure 6 Workflow Studio, the current A+W iQuote workflow has to be loaded with the extension point "0000 - A+W iQuote". There, you open the workflow core area. Now you see the complete workflow and scroll down and at the end of the workflow, there is the element `"ValidatorItemRemarks"`, on which you click. The properties are loaded in the right area of the Workflow Studio. There, you set the property `"ShowInCart"` to True.

> **UI Screenshot: ValidatorItemRemarks Properties**
> The properties pane for the `AWSOA.Web.Configurator.Services.Workflows.ActionValidatorltemRemarks` activity is shown. The `ShowInCart` property is highlighted and set to `True`.

Save change and restart the infrastructure services in the service locator, as well as the A+W iQuote services.

## 15.6. Images for A+W iQuote

### 15.6.1. Product images

In A+W iQuote, standard images are drawn as default if no image was stored. These standard images are delivered with A+W iQuote (`C:\SANDPIPER1\WebWeb\Content\auw\products`) and assigned with the article type (`artikel.atyp`):

- `FLOAT_FM` atyp=100 → `"1004.png"`
- `ESG` atyp=150 → `"4004.png"`
- `VSG_FM` atyp=170 → `"6012.png"`
- `ISO` atyp=200 → `"150000.png"`
- `ZUBEHOER` atyp=800 → `"14200.png"`
- `RAHMEN` atyp=210 → `"12006.png"`

No assigned image causes application of `"none.png"`.

In A+W Enterprise, the product images can be maintained on the article master data dialog (Master Data > Articles > [Shift+F4] > Article Images).

The A+W Enterprise image path that is used for this dialog is stored in the environment variable `"ARTIKELBILD_PFAD"`.

> **UI Screenshot: Article Images Master Data**
> The master data screen for an article shows the "Artikelbilder" (Article Images) tab. The "Anzeige" (Display) field is set to "Online", and a path to a "door.png" file is specified.

For maintenance of the A+W iQuote images, the display data field must be set to the new value `"Online."` When this has happened, the data field "Position in the image" is grayed out since this data field is irrelevant for the A+W iQuote. In the data field path, the desired image must be specified via path or searched for via the Explorer, with [F9]. It is only possible to maintain .PNG image files.

So that the images that are maintained in A+W Enterprise are available in A+W iQuote, the images must be copied to the desired subdirectory of the A+W iQuote. The default directory is `"\Content\auw\products\"`. For the customers, it makes more sense to create a new subdirectory in which the product images are stored, for this default directory is overwritten in the update process; the subdirectory remains. So that A+W iQuote knows the correct subdirectory for the individual products, the workflow must be adjusted and the property `"Content/Image"` in the area of the product widgets. There by default, `"auw/product"` is stored and can be adjusted.

### 15.6.2. Images for product groups

In order to assign the respective product groups appropriate images, you have to store the required images in the `"\Content\auw\productgroups\"` directory. So that the images are assigned to the correct groups, you have to rename the image file with the short name of the article groups (Master Data > Keys > Products > A+W iQuote-specific details > Article groups).

> **UI Screenshot: Article Groups for A+W iQuote**
> A table shows the configuration for A+W iQuote article groups. It lists the Number (Nr), Language (Spr), Short Name (Kurzbezeichnung), and Text for each group.
> | Nr | Spr | Kurzbezeichnung | Text |
> |----|-----|-----------------|-------------------------|
> | 1 | 1 | Bearbeitungen | A+W iQoute Bearbeitungen |
> | 100 | 1 | FLOAT | Float |
> | 150 | 1 | ESG | ESG |
> | 170 | 1 | VSG | VSG |
> | 200 | 1 | ISO | ISO |
> | 300 | 1 | FIX | Doors |
> | 830 | 1 | Products | Products |

For example, you have a file `"xyz.png"` for the float group and rename this file `"FLOAT.png."` If you now move this file into the `"\Content\auw\productgroups\"` folder, this file will now be displayed as group image.

## 15.7. Colors and variants

For the colors and/or variants, AWE master data, as well as adjustments to the A+W iQuote workflow must be made.

Size variant was developed under ticket [AW-153568].

### 15.7.1. Master Data

**Color**

The colors (hardware parts) for articles are maintained on the item master data dialog (Master Data > Item > Phys. Properties) in that you set the toggle data field `"Color/size variants"` to color.

> **UI Screenshot: Article Master Data - Physical Properties for Color**
> The physical properties tab for an article is shown. The "Farben-/Größenvariante" (Color/size variants) toggle field is highlighted and set to "Farben" (Colors).

The individual colors can be set on the submenu ([F4] key in the article master data) `"Colors/sizes"`.

So that the selection possibilities for the colors in A+W iQuote are displayed in color, the RGB values of the colors used must be maintained in the database table `xxfarbe`; otherwise the areas will be displayed in black.

The RGB values must be maintained under `"Master Data > Keys > Products > Variants > Colors > Colors."`

**Dimensional variant**

The variants for articles are activated on the article master data dialog (Master Data > Item > Phys. Properties) with the `"Maßvariante"` flag.

> **UI Screenshot: Article Master Data - Physical Properties for Variant**
> The physical properties tab for an article is shown. The "Maßvariante" (Dimensional variant) flag is checked.

For the variants, the flag `"Maßvariante"` must be active and for the colors, the toggle data field `"Colors/size variants"` must be on colors. **Both possibilities cannot be active at the same time.**

The individual variants can be set on the submenu ([F4] key in the item master data) `"Variants"`.

**Size variant**

The size variants for articles are maintained on the item master data dialog (Master Data > Item > Phys. Properties) in that you set the toggle data field `"Color/size variants"` to sizes.

> **UI Screenshot: Article Master Data - Physical Properties for Size**
> The physical properties tab for an article is shown. The "Farben-/Größenvariante" (Color/size variants) toggle field is highlighted and set to "Größen" (Sizes).

The individual sizes can be set on the submenu ([F4] key in the item master data) `"Colors/sizes."`

### 15.7.2. Appearance of the selection possibilities in A+W iQuote

The selection possibilities of the colors can be designed in terms of their color with the above-mentioned RGB values from the master data.

> **UI Screenshot: Color Selection in iQuote**
> The UI shows a color selection panel with different colored squares representing available colors like "silber", "niromatt", "verkehrsweiss", etc.

The dimensional variants are specified with a blue tone as default selection area.

> **UI Screenshot: Variant Selection in iQuote**
> The UI shows a variant selection panel with different sized rectangles representing available dimensional variants like "450.0 x 321.0", "510.0x321.0", etc.

The size variants require the maintenance of article images.
An image can be stored for all 3 variants. These images must be stored under the respective content paths (to be set up in the respective validators in the workflow) and have as image names the variant no. (`var.bitnr`) and the color no. (`artfarbzu.farbnr`).

> **UI Screenshot: ValidatorColors Properties**
> The properties pane for the `ValidatorColors` widget is shown, with the `ContentPath` property set to `"auw/products"`.

To be heeded is that the numbering of the colors/sizes and dimensional variants in the AWE database tables are frequently the same and if you activate both possibilities, two different content paths should be set up for the different validators.

### 15.7.3. Workflow

> **Note:** Please heed when setting up the variants and colors that `AutoSelect` in the properties is set to true. Otherwise it can happen that the newly selected article has an old color or variant stored.

**Colors**

So that product colors can be selected in A+W iQuote, the 0000 – A+W iQuote workflow used must be adjusted. For this, in Workflow Studio, you load the workflow used and drag the Product Colors widget (ValidatorColors) onto the loaded workflow. The widget is on the left of the selection area.

> **UI Screenshot: Adding ValidatorColors Widget**
> The Workflow Studio shows the "iQuote Glass" toolbox with the "Product Colors" widget highlighted. The properties pane for "ValidatorColors" is on the right.

The `ValidatorColors` widget offers some setting possibilities (see configuration instructions EN-CONFIG-A+W iQuote).

New for the setting possibilities is the **ColorCode**; this data field expects a created variable (here: `colorCode`). If this variable has not yet been created, it should look as follows:

> **UI Screenshot: Variables Tab**
> The variables tab in the workflow designer shows a list of variables. The `colorCode` variable is highlighted, with type `String` and scope `Workflow Core`.

The dialog for this is displayed as a tab at the bottom left on the loaded workflow.
Attaching the product colors widget after the ValidatorProduct and filling out of the properties of the product color widget are sufficient to configure the colors for articles.

**Dimensional variant**

So that size variants can be selected in A+W iQuote, the 0000 - A+W iQuote workflow used must be adjusted. For this, in Workflow Studio, you load the workflow used. The `ValidatorColors` are also used for the dimensional variants. You drag the product colors widget (ValidatorColors) onto it. The widget is on the left of the selection area.

The `ValidatorColors` widget offers some setting possibilities (see configuration instructions EN-CONFIG-A+W iQuote).

New for the setting possibilities is the **ColorCode**; this data field expects a created variable (here: `colorCode`). If this variable has not yet been created, it should look as follows:

> **UI Screenshot: Variables Tab (again)**
> The variables tab is shown again, highlighting the `colorCode` variable of type `String`.

The dialog for this is displayed as a tab at the bottom left on the loaded workflow.

The dimensional variants use the same widget as the colors and therefore, configuration is a bit different.

> **UI Screenshot: Workflow Logic for Variants**
> A workflow diagram shows an "If-Variante" condition. In the properties for the `ValidatorVars` activity, the `ProductNoIn` property is set to `-1*productid`.

The difference between variants and colors is the last data field (`ProductNoIn`). In the variants, the product number is handed over as a negative to the documentservice so that we can distinguish between color and variant. The `Product No.` of the colors/hardware is always positive.

**Size variant**

So that size variants can be selected in A+W iQuote, the 0000 - A+W iQuote workflow used must be adjusted. For this, in Workflow Studio, you load the workflow used and drag the `Product Size Variants` widget (`ActionValidatorSizeVariants`) onto the loaded workflow. The widget is on the left of the selection area.

> **UI Screenshot: Adding ActionValidatorSizeVariants Widget**
> The Workflow Studio shows the "iQuote Glass" toolbox with "Product Size Variants" selected. The properties for `ActionValidatorSizeVariants` are displayed, showing fields like `AutoSelect`, `Category`, `ContentPath`, and `ProductNoln`.

The `Product Size Variants` widget is attached in the workflow and is filled out similar to the image above.

**BOMs colors**

It is now possible to activate the colors for a search on the BOM level.

> **UI Screenshot: ValidatorColors Properties for BOM**
> The properties pane for `ValidatorColors` is shown with the `IsBomColor` property highlighted and set to `True`. The `Category` is set to `"Size Variant"`.

This possibility was created in order to combine dimensional variants with colors. (Ticket [AW-153568]). The dimensional variants are, as described above, set up and still drawn from the header article. That is, from the article that is visible on the A+W iQuote article selection. The additional BOM colors, set up with the new property `IsBomColor`, are drawn from the first article of the header article BOM, which has set `artikel.farbflag=1`.

## 16. Order release

All online orders (A+W Enterprise iQuote) are not released directly; instead, they are put in the release pool.

For further information, see "EN-CONFIG-A+W Enterprise" section "Release pool".

For online entries in the call center, see "EN-CONFIG-A+W Enterprise Internal Client Separation" section "Call center solution" and "EN-CONFIG-A+W Enterprise" section "Release pool"

## 17. Orders in the call center

In the default configuration, A+W iQuote orders that are entered in the CALLCENTER are assigned directly to a client. If this should not be the case, this must be configured via a global environment variable.

`IQUOTE_CALLCENTER_STAY` (client reference: no)

If this environment variable is active, online orders (entered in A+W iQuote) that are entered in the CALLCENTER remain in the call center. There is no automatic site assignment.

(see also "EN-CONFIG-A+W Enterprise" section "Release pool")

## 18. Status

For the A+W iQuote orders and quotations, individual status messages are sent in the course of running through the system.

This development was updated with DevOps item #92808.

The following table describes the status displayed in the order and quotation history.

| Processing name | Number | Description |
| :--- | :--- | :--- |
| Document created | 900 | Document was entered successfully in A+W iQuote and transferred to A+W Enterprise. |
| Document reworked in A+W iQuote | 901 | Document was changed in A+W iQuote. |
| Document entered in A+W Enterprise | 902 | Document was entered in A+W Enterprise and is now visible in the document overview. |
| Document reworked in A+W Enterprise | 903 | Document was changed in A+W Enterprise. |
| Order confirmation generated | 904 | Order confirmation was generated. |
| In production (in processing) | 910 | Document was transferred to production. (No individual steps are listed) |
| Delivery is underway | 940 | Document was released for delivery. |
| Invoice issued | 950 | Invoice for the document was issued. |
| Credit note created | 960 | Credit note for the document was created. |
| Cancellation of the document | 990 | The cancellation of the document was initiated. |

The data is saved in the table `kaufstat`.

Status 910 - "In processing" is generally set for all messages from A+W Production or other modules if for the order the general status messages are sent: from Status= 300 (fixed) to status 302 (released) and for all Status>502.

If you would like to activate the status display for all A+W Enterprise orders (also not online), you can achieve this with the ENV configuration: `IQUOTE_ALL_CUSTOM_STATUS = ON`.

## 19. Okta Login Page

The Okta login page was developed under ticket [AW-158578], it is an upstream login page and independent of iQuote. On it, the user logins are managed; users can register themselves. The user is assigned an iQuote instance.

The standard login process for iQuote is thus overwritten and replaced with a one-time token and previous system comparison check. It is not possible to use both login variants at the same time.

The login page and the iQuote have a trust relationship that is secured with a private key and permitted IP addresses. Only if the private key is the same in both systems and the requesting IP address is permitted in the back end do the systems trust one another. A user who has authenticated himself on the login page is thus authenticated in iQuote with a one-time token.

> **Diagram: Okta Login Flow**
> A diagram shows the interaction between the Login Page, iQuote, and the Okta Tenant.
> 1. Login page sends a "Token request" to iQuote.
> 2. iQuote sends a "Token send" back.
> 3. The user performs a "Login + call".
> 4. Redirects like "Login Challenge redirect", "Signin redirect", and "SignOut redirect" happen between the Login Page and the Okta Tenant.
> 5. iQuote has "Token storage".
> 6. The Okta Tenant stores "User Credentials".

For the Okta login page, it is necessary that the customer creates an account with www.okta.com and creates user master data there, similar to how the customer does with the back end active directory for A+W Enterprise.

### 19.1. Installation

Via the A+W SetupLauncher, the **A+W iQuote 6 Login Okta** diskset under `A+W Common` and the **Microsoft.net 8.0.0 – Windows Server Hosting** diskset under `External Software` must be selected.

The installation should, like the A+W iQuote 6 Web (front end) be done on a Web server that is in the DMZ (demilitarized zone).

Since Okta is not hosted locally, there must be internet access on the Web server so that there can be communication with the Okta account.

> **UI Screenshot: A+W SetupLauncher**
> Two screenshots of the A+W SetupLauncher's "Component Selection" screen. The first shows "A+W iQuote 6 Login Okta" selected. The second shows "Microsoft.NET 8.0.0 - Windows Server Hosting" selected under "External Software".

The remaining components (iQuote Web, iQuote Services, Infrastructure 6 Services, Infrastructure 6 Web and Documentservice) must be from QR [2403] or newer.

### 19.2. Configuration

The configuration requires an Okta account, which the customer must have created in advance and support. We will probably not have access to this account and therefore it is important that we have a direct contact person during the setup of the system.

#### 19.2.1. Okta platform

Using the Terraform tool, it is possible to use a superior configuration language to bring a cloud or the local infrastructure into the desired state for execution. Thus, we must first download the command line tool from [Terraform by HashiCorp](https://www.terraform.io/).

Unpack the tool (`terraform.exe`) and place it together with the folder (`C:\SANDPIPER1\WebLoginOkta\Okta`) in a secure place (e.g., `"C:\Okta"`). This is necessary since after executing the tool, a state screen for the Okta configuration is created. This may not be lost, which can happen after a diskset update.

Now we configure the `okta.tf` file in the new directory in order to import an update of the configuration. We open the `okta.tf` in Notepad.

Now we need information from the customer's Okta account.

The customer must generate a token that allows Terraform to make changes to the Okta tenant. A new token is created for this in the Okta admin panel on the left menu under `"Security->API"`. Make sure that the token is copied directly after creation.

> **UI Screenshot: Okta API Token Creation**
> The Okta admin dashboard shows the API section. A dialog "Token created successfully!" displays a token value and warns that it will only be shown once.

This token must be entered in the `"okta.tf"` file under the `"api_token"` element. For the `"org_name"` and `"base_url"`, see the Okta admin panel.

> **UI Screenshot: Okta Admin Panel Header**
> The header of the Okta admin panel shows the user's name and the organization URL, e.g., `dev-54857752.okta.com`.

`"dev-54857752.okta.com"` is divided into `org_name` and `base_url` and changed directly in the `okta.tf` file. Example:

```
provider "okta" {
  org_name = "dev-54857752"
  base_url = "okta.com"
  api_token = "<TOKEN>"
}
```

In addition, the URL that points to the "A+W Web Login Okta" must be adjusted with `https://`. Example `WEB_LOGIN_HTTPS_URL` from test system `aweawpvnext`: `"https://aweawpvnext.tse.intra/Web.Login.Okta/"`

```
variable "WebLoginUrl" {
  type = string
  default = "https://aweawpvnext.tse.intra/Web.Login.Okta/"
}
```

Now we open a command line (Windows + r, enter `"cmd"` and OK).

In the command line, you navigate to the created folder `"C:\Okta"` with the following command.

```bash
cd C:\Okta
```

After we are in the correct folder, we use Terraform to configure Okta. This is done in the same folder via the command line using the following commands:

```bash
terraform init
terraform plan
terraform apply
```

According to `"terraform plan"` the information from the `okta.tf` is listed. Check this information and then confirm with `"Yes"`.

If the terraform has been executed successfully, you will find the application in the Okta account under `Applications > Applications`.

> **UI Screenshot: Okta Applications List**
> The Okta Applications page shows the newly created "iQuote" application.

#### 19.2.2. A+W iQuote Login Okta

To switch the new login page live, the "A+W iQuote Okta Login Page" of the Okta tenant must be made known. This is done with the configuration file `"C:\SANDPIPER1\WebLoginOkta\appsettings.json"`. The `"Okta"` rubric must be configured in this file.

```json
"Okta": {
  "OktaDomain": "https://<OKTA_TENENT_HERE>.okta.com",
  "ClientId": "<CLIENT_ID_HERE>",
  "ClientSecret": "<SECRET_HERE>",
  "AuthorizationServerId": "default",
  "UseRedirectModel": "true"
},
```

For `"OktaDomain"`, see the Okta admin panel as depicted in the figure. Important is that `https://` is placed in front of the Okta domain.

For the `"ClientId"` and `"Clientsecret"`, use the left menu to navigate to `Application > Application` and selecting the `iQuote` application. Here, the values can be viewed as in the figure and entered with the Copy button.

> **UI Screenshot: Okta Application Client Credentials**
> The "Client Credentials" section for the iQuote application in Okta is shown. It displays the `Client ID` and `Client Secret`, with buttons to copy them.

In the `"Clients"` area in the JSON file, the private key for the client in question must be stored. For the `clientID`, see the A+W Infrastructure Web. Or if the clients for the iQuote configuration should be clarified and listed here.

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

The private keys must be stored here and in the environment variables of the A+W Enterprise of the respective client.
Environment variable: `IQUOTE_LOGIN_PRIVATEKEY`

**CAUTION:** A private key must be compared between the login page and A+W Enterprise; otherwise no connection can be established. Leaving this blank is not an option.

In addition to the private key, the IPv4 or IPv6 address of the login page server must be entered here. Only queries from this computer are permitted.
Environment variable: `IQUOTE_LOGIN_REMOTE_ADDRESSES` (Separated with semicolon)

**Caution:** You must absolutely also store the IPv6 (`":::1"` is the local host here).

To apply the configuration of the JSON file, the `"Web.Login.Okta"` page in the IIS manager must be restarted.

> **UI Screenshot: IIS Manager Restart**
> The IIS Manager is shown with the "Web.Login.Okta" site selected. The "Restart" action in the right-hand pane is highlighted.

#### 19.2.3. Preparation of iQuote for the Okta login

In the Infrastructure Web, the logout detour to the login page must be configured:

> **UI Screenshot: Infrastructure Login Configuration**
> The "Login configuration" section in the A+W Infrastructure settings is shown. The "Log out redirect URL" is filled with the Okta sign-out URL, e.g., `https://aweawpvnext.tse.intra/Web.Login.Okta/Account/SignOut/`.

Under the element `"Log out redirect URL"`, the web address of the login page must be entered. Important here is that the extension of the URL includes `"/Account/SignOut"`.

**NOTE:** The `"Okta"` rubric point can be ignored initially since it does not contain any function.

To apply the configuration, the `"Web.Web"` page in the IIS manager must be restarted.

> **UI Screenshot: IIS Manager Restart (Web.Web)**
> The IIS Manager is shown with the "Web.Web" site selected. The "Restart" action is highlighted.

#### 19.2.4. Customization

As "deployment model", "A+W iQuote Login Okta" relies on the Okta redirect model. [See here](https://developer.okta.com/docs/guides/redirect-authentication/) to learn more about this. This means that the entire customization happens via Okta itself; see also [Style the sign-in page | Okta Developer](https://developer.okta.com/docs/guides/style-the-widget/).

### 19.3. Okta data maintenance

The following data maintenance must be done by the customer, unless the customer gives you the login for his Okta account. For the data maintenance on the Okta page, the A+W iQuote users must be stored in the Okta account.

Tip: If you create data in the Okta interface and it is not displayed right away, you must wait a few seconds and then refresh the window. Frequently, the display of the data is a bit delayed.

#### 19.3.1. Group

Under `Directory > Groups`, use the `"Add Group"` button to create the groups.

> **UI Screenshot: Add Group in Okta**
> The "Add group" dialog in Okta is shown. A user is entering a group name ("iQuote 140") and an optional description.

First the group name is specified. A description can improve the clarity of the group later on.

After saving, select the group on the list.

Under Application, the `iQuote` application must be added that we imported into the configuration via Terraform (19.2.1 Okta Platform).

> **UI Screenshot: Assign Applications to Group**
> The dialog to assign applications to the "iQuote 140" group is shown. The "iQuote" application is selected.

You will also be asked for additional information. Here, you enter the Web address to which the redirect should happen if the user has logged in successfully. In our example, this is the test systems of AWEAWPVNEXT with the client number 140. Finished.

> **UI Screenshot: Assign Application with SiteURL**
> An additional information dialog asks for a "SiteURL". The URL for the specific client is entered, e.g., `http://aweawpvnext.tse.intra/Web.Web/140`.

#### 19.3.2. User

The users created need an A+W Enterprise employee with assignment to a market partner. The master data maintenance is under 4.2.1 Okta Login Page.

Under `Directory > People`, use the `"Add Person"` button to create the users.

> **UI Screenshot: Add Person in Okta**
> The "Add Person" dialog is shown, with fields for First name, Last name, Username, Primary email, and Groups.

It is possible to add users compressed via .CSV file (under `"More actions"`).

A group can be assigned to the user. You can add groups to a user later on. To simplify the flow, it makes sense to create the group(s) first.

The activation can be selected whether you would like to activate the customers directly or after the fact.

Passwords can also be specified. This is a decision that the customer must make, whether he would like to specify passwords.

If the user is saved, this user is sent an e-mail in which he is asked to verify his account and set a password if necessary.

These created users require their appropriate market partner number, which was maintained in A+W Enterprise. For this, select the individual user under `Directory > People`. So that the market partner number can be maintained, the user must be assigned to a group that owns an application. In our example, we added a group directly when creating the user and thus see the required application and from which group this application is drawn.

> **UI Screenshot: User's Assigned Applications**
> A user's profile page shows the "iQuote" application assigned to them via the "iQuote Users" group.

With the pen button on the right side, the editing mode is opened for this user. After scrolling down, the market partner number maintained in A+W Enterprise is entered under `ERPCustomerID`.

The `SiteURL` from the group is also displayed here. If no groups are used, you must store a Site Url for all users and link the users individually with the application.

> **UI Screenshot: Edit Application Assignment for User**
> The editing dialog for a user's application assignment is shown. The `ERPCustomerID` field is visible and has a value entered ("133700"). The `SiteURL` is also displayed.

## 20. Restrictions

### 20.1. Input

**Purchase order**

PO items can only be entered without restriction violation. It is not possible to place articles in the A+W iQuote shopping cart that have a price error, for example. If it happens that an article violates a restriction, the Add button in A+W iQuote is switched off. This gate was incorporated in order to make sure that no POs are entered that can be saved automatically in the system with zero prices or similar violations.

> **UI Screenshot: Price Error Message**
> A message is displayed: "Der Preis für das gewünschte Produkt konnte nicht ermittelt werden." (The price for the desired product could not be determined.)

**Purchase order request**

PO request items can be entered with restriction violations. These items can be added to the shopping cart without a problem and the PO request can be entered completely. This is permitted since these inquiries will always have to be reworked by an employee.

If an incorrect PO request is given, then the market partner assigned to the revenue (`mp.vertrerloe`) is sent an e-mail.

### 20.2. Processings

The restriction check for the processing parameters can be activated with `IQUOTE_WITH_PPARAM_TEST`. This is also how the test for the double processed edges/corners is activated.

For the processings stored in the A+W iQuote, it is possible to set that the restriction check is also not displayed for non-existant values. Set-up is done using the environment variable `IQUOTE_LEERE_BEARB_MELDEN`.

For more precise information, read the chapter: Master data consolidation > Article master data > Processings.

### 20.3. Glass

It must be noted that a product release of a non-fixed glass for the A+W iQuote always requires a geometry validator. If there is no geometry validator in the workflow, then no dimensions can be specified and thus no SN sketch will be displayed.

[AW-158039] // October 2023

In A+W Enterprise iQuote, dimension restrictions are generally executed only on the product level, not the BOM level. If necessary for IGU products that the dimension restrictions of the glass be tested on the 1st level of the BOM, this can be done with an environment configuration.

`IQUOTE_IGU_TESTLEVEL` (client reference: no)

By default, A+W Enterprise iQuote checks the dimension restrictions only on the product level. If the variable is activated and
= 1: For IG, the restriction check can be expanded to the 1st level (glass).

### 20.4. Incorrect or locked quotations/PO requests

If a conflict in the entry of a product in A+W iQuote is determined, then this product can only be saved as a quotation that should be examined after the fact. In A+W iQuote, you generally make a distinction between the following types of conflicts for quotations:

- Restrictions (dimension or processing parameters)
- Price
- Restrictions + price

These quotations get a lock info record in the table `kaufstat` with corresponding status (max. of all items)

- **800** - Restriction violation
- **801** - Pricing error
- **802** = 800 + 801

> **UI Screenshot: Conflict Message in Quotation**
> A quotation entry screen shows a conflict message at the top: "KONFLIKT: Maß-/Parameter Restriktionen" (CONFLICT: Dimension/Parameter Restrictions).

In addition, the items also get an expanded individual error status (`kposstat`):

- **800** - Dimension restriction violation
- **801** - Pricing error
- **802** = 800 + 801
- **803** = Processing parameter missing or restrictions of the Bearb.Parameter violated
- **804** = 800 + 803
- **805** = 801 + 803
- **806** = 800 + 801 + 803

> **UI Screenshot: Conflict in Item Position**
> The item list in a quotation shows a conflict message for a specific item: "KONFLIKT: Bearbeitungsparameter" (CONFLICT: Processing parameters).

As long as there is a lock due to an error status on a quotation, this quotation cannot be transformed into an order via A+W iQuote. This action can only be performed directly in A+W Enterprise.

The lock status can be eliminated by the check in A+W Enterprise. The problem quotations must be viewed and unlocked under a new menu element `Sales > Quotation check > Online quotations`.

> **UI Screenshot: Online Quotations Overview**
> A list of "Online Angebote" (Online Quotations) is shown. Each has a status and a remark, such as "Fehlerhafter Preis" (Incorrect Price) or "Fehlerhafte Restriktionen" (Incorrect Restrictions).

There are also various possibilities for releasing the quotation.
1.  With `<Sh+F5>` or the `"Quotation"` button, you can enter the quotation in the document entry. Here, you can check and adjust the quotation. When saving the change, the question is asked whether the lock status should also be removed.
2.  If no changes must be made, then you can eliminate the lock and save the quotation directly via `Ctrl+F` in the quotation footer.
3.  The removal can be implemented directly from the overview by setting the release to yes and performing the action with `<F3>` or the `"Release"` button.

The records from the tables `kaufstat` and `kposstat` with status of 800 to 807 are deleted and in the fields `kauf._kontrollmanr` and `kauf._kontrolldate` are assigned. The field `kauf._kontrollmanr` contains the employee number of the user and `kauf._kontrolldate` the current date.

## 21. Troubleshooting

Here is a list of all known problems that can occur and be eliminated during the configuration of A+W iQuote.

### 21.1. License server

#### 21.1.1. No connection to the license server

If the A+W iQuote is loaded without selection possibility after log-in, it could be that the problem is a missing license for A+W iQuote or that the connection to the license server has failed.

> **UI Screenshot: A+W iQuote Blank Screen**
> The main A+W iQuote screen is shown empty, without any product selection options, indicating a loading or connection issue.

To check whether the license server is reached, you can go to `"C:\ProgramData\Microsoft\Windows\Start Menu\Programs\A+W\Config Tools"` and start the link `"A+W LicenseClient Machine Settings Config Tool"` and test the connection. After you have clicked the Test button and the tests were successful, a message box is displayed that confirms the successful test. After that, press `"Next"` until the configuration is complete.

> **UI Screenshot: License Client Configuration Tool**
> The configuration tool shows options for connecting to a license service. A user can specify if the service is on the local machine or another machine, and enter the host name or IP address.

It can happen that the name resolution is not recognized; then the IP address of the license server should be entered.

#### 21.1.2. License expired

The same scenario occurs if the A+W iQuote license has expired.

To check the license, the `A+W LicenseServices Monitor` must be opened on the Start menu and the license on the desired server sought under `"Application: A+W Sandpiper (2400)"`.

> **UI Screenshot: A+W License Monitor**
> The license monitor shows a tree view of licenses. It displays the license for "Application: A+W Sandpiper (2400)" and its modules, like "iQuote Configuration".

Example of the multisite fair text environment.
Important: IIS must be restarted, otherwise the license is not obtained anew.

### 21.2. Problems with zero workflows and predefined workflows

It happened increasingly that the set workflows were no longer detected correctly in the Workflow Studio after an update of the front-end components of A+W iQuote.

In the WebConfigurator log, there is then an error message that the workflow used may not be `"zero."`

If this problem occurs, then you can add the installed workflow again via the XAML file and reinstall it. After that, the workflow should be recognized again.

Unfortunately, we do not understand what causes this error. If this error has occurred once, please let Development know and if necessary, back up the A+W iQuote Services so that we can research the issue.

### 21.3. No images in the IG exchange BOM

It can happen that the drawings in the IG BOM are not displayed properly. The following sample image shows the missing inner spacer.

> **UI Screenshot: IG Exchange BOM with Missing Image**
> The IG exchange screen shows a diagram of an insulated glass unit. The inner spacer is missing from the drawing.

The drawings and images on the IG exchange or muntin exchange screen depend on the master data adjustments under 20.6.2 Produkte. It is important that the glass, spacers, gases, and muntins that are used and are in the BOM of the insulated glass always have to be on `+online` in the article master data.

Similarly, for the inner spacer a standard AIR has to be maintained since the iQuote user has no opportunity to enter an AIR. If in the IG article `"mandatory dimensions"` were maintained, then a record for the AIR has to be maintained there and a value specified. Otherwise you will see the error image mentioned above.

> **UI Screenshot: Mandatory Dimensions Master Data**
> The master data screen for an article's mandatory dimensions is shown. This is where the standard AIR value would be set.

### 21.4. Problems during loading/opening of workflows in Workflow Studio

It happens again and again that the following error is displayed in Workflow Studio if you try to load a workflow via XAML or from the database.

> **Error Message: Workflow Designer encountered problems**
> `! Workflow Designer encountered problems with your document`
> `Please check the document for invalid content, namespaces, references or reference loops.`
> `'The type 'InArgument(awcs:ConfiguratorCore)' of property 'Configurator' could not be resolved.' Line number '3' and line position '37'.`

Please set the correct reference path to the installation location of the A+W iQuote/Web Configurator in Workflow Studio under `"Configuration > Settings > Reference paths"`. (20.8.1 A+W Infrastructure 6 Workflow Studio)

> **UI Screenshot: ConfigurationDialog - Reference Paths**
> The dialog for setting reference paths in Workflow Studio is shown. A user needs to add the folder path to the WebServices\Configurator installation.

When entering/changing the path, confirm with the Update button; otherwise you will exit the dialog without saving.

When checking the path, please pay attention that the desired service, here the `Configurator`, is actually installed in the reference path. The Workflow Studio requires the service to open the workflow.

A customer had split his system so that the WebConfigurator was neither installed on the process server of the infrastructure nor on the service of the iQuote front end, but rather on a third system. And only on the third system was it possible to open the workflow for A+W iQuote via the Workflow Studio.

If the following error occurs, the Workflow Studio version might be too old and it must be updated.

> **Error Message: Unhandled Exception**
> `An unhandled exception occurred, see log for details: Could not load type 'AWSOA.Core.Contracts.Interfaces.IceDeployment.liceGridAdmin' from assembly 'AWSOA.Core.Contracts, Version=13.2.114.0...`

### 21.5. No database connection on the host server of the A+W infrastructure

For one customer, there were connection problems from a separate A+W iQuote server in the direction of the host server where the rest of the A+W infrastructure (here the A+W Production Server) is installed. A database problem was reported in the logs of the Web.Configurator. There was supposed to be no correct connection string for connection.

This problem was eliminated with installation of an A+W infrastructure web on the A+W iQuote server. Normally for a separate installation of A+W iQuote, only an A+W infrastructure middleware should be required; however somehow this was not sufficient.

### 21.6. No dispatch of the OC possible

At one customer [AW-102433] there was a case where the entered A+W iQuote order could not be printed. The reason for this was a missing department number for the user (`kauf.abtnr`). Since the A+W iQuote creates the orders as the user system, as with `intauf`, that is, with employee number -1, no department number is assigned.

So that a department number is entered nonetheless, the environment variable `INTAUF_ABTNEU` must be set.

### 21.7. Web Configurator does not start or timed out

The behavior can occur that the Web Configurator service crashes when starting. This behavior can be detected in the Service Locator if the desired service is displayed for too long with the green plus sign and goes out after that.

> **UI Screenshot: Service Locator Service List**
> A list of services shows the status of various A+W components, such as `AWEAWPVNEXT-Web-Configurator-140-001`.

In the `Web.ConfiguratorService` log, the following exception should be found:

> An inner exception occurred:
> Type: System.Net.Sockets.SocketException
> Message: A connection attempt failed because the connected party did not properly respond after a period of time, or established connection failed because connected host has failed to respond

Similarly, you can see the failed generation attempt of the proxy creation of the Unix service, here document service, in the log:

> Inner Exception Message: " | "
> An exception occured:
> Type: AWSOA.Core.Exceptions.CoreCommunicationException
> Message: Ice.ConnectFailedException while executing method 'DocumentService Proxy create'

Due to the communication from the Windows in the direction of Unix, this behavior is very probably caused by a blocking firewall on the Unix system. As a test, you can switch off the firewall and try to start the services. For a customer-oriented solution, the port of the Web.Configurator must be released on the Unix system in the firewall. This will very probably be done by the customer-internal IT.

### 21.8. Duplicate key when saving a workflow

With one customer, we had the problem that the saving of a workflow via the Infrastructure.Web caused an error.

After checking the trace file (`Infrastructure.Web_xxx.awtrc`), we noticed the following database error.

> 2024-04-22 12:29:29.283 | [12304] | [0x00000023] | ERROR | Core |
> Update workflow assignment | Workflow WebConfigurator Enterprise Groups Extended_new.xaml / ExtensionPoint WebConfigurator | "Error Code 1000522, Message: Duplicate key in database: ERROR [23000] [Informix][Informix ODBC Driver][Informix] Could not insert new row - duplicate value in a UNIQUE INDEX column (Unique Index:ui_wfactivityassignments01). " | "

An exception occured:
> Type: AWSOA.Core.Exceptions.Data.CoreDataDuplicateKeyException
> Message: Duplicate key in database: ERROR [23000] [Informix] [Informix ODBC Driver] [Informix] Could not insert new row - duplicate value in a UNIQUE INDEX column (Unique Index:ui_wfactivityassignments01).

In the underlying Informix database, some GUIDs in the table `Core_WFActivityAssignments` column `Guid` were entered in capital letters.

The GUIDs in the Informix table must be entered with lower-case letters.

The updating of the entries to lower-case letters corrected the problem.

### 21.9. General performance problems

Under ticket [AW-220650], a lot of research has been done to improve the performance for customers. The settings found were taken over into the installation instructions EN-INST-A+W Enterprise iQuote. Please read it for the steps for system configuration.

## 22. Search/service

### 22.1. Logs

You can learn about setting up the logs in the EN-CONFIG-A+W Enterprise System.

#### 22.1.1. Price report

The price log is always written regardless of a configuration. It is in `$PROTOPFAD` in the backend (possibly under the client directory) and is called `"WebPr<mmdd>"`. Here, all messages are logged that are normally output in the foreground and cause a "price error" in iQuote.

### 22.2. General

You can find a listing of all ICE services in the `"Service Locator Administration"` Tool, which is in the Config Tools folder of the Desktop A+W folder (`C:\ProgramData\Microsoft\Windows\Start Menu\Programs\A+W\Config Tools`). Here you can see in compact form how all services run together.

If you open the tool, you can see the set connections with a click on the button with the green arrow in the upper left corner.

> **UI Screenshot: IceGrid GUI - Saved Connections**
> The IceGrid GUI tool is shown, with a saved connection `AWRegistry:tcp -h "localhost" -p 12000` selected.

Establish the connection, and after that, you will see the following list:

> **UI Screenshot: Live Deployment Runtime Components**
> A tree view shows the runtime components, organized by node. Example nodes are `MULTISIDE-FAIR-CAD` and `VMAUWX-Commercial-20`.

I will use this list as an example.
First we see the following: `MULTISIDE-FAIR-CAD`. This point is called a node and has the notation `<computer name-service area>` = Multiside-fair is the computer and CAD, the service area, where particular CAD services can be found.
For the AWE Backend, we see that a Unix computer is entered with `VMAUWX`.

In Windows, a node reflects precisely one Windows service (marked in yellow):

> **UI Screenshot: Windows Services List**
> A list of local Windows services is shown. Services like `A+W CAD 6`, `A+W CIM 6`, and `A+W Commercial 6` are highlighted, corresponding to the service nodes.

On Unix or in the Backend, the running `icegridnode` is next to the node:

```bash
wmauwx 20:/alcibprg1/gb:psgrep icegrid
JID      PID PPID C STIME TTY      TIME CMD
awserv 25467 47402 0 16:28 pts/0    00:00:00 psgrep icegrid
alhi20 56576   1   0 10:57 ?      00:00:00 icegridnode --Ice.Config=/alcibdat/20/preise/ices/config.node
```

If a Windows service or the `icegridnode` should be deactivated, then the little hard disk in the service locator administration turns red:

> **UI Screenshot: Service Locator with Red Indicator**
> The runtime components view shows a red hard disk icon next to a node, indicating it is down.

The actual services are below the nodes. If these services are switched on, they have a little green triangle.
Notation: `<computer name-service area-service name-client>`

### 22.3. Which services are affected for A+W iQuote?

The relevant services for the A+W iQuote are the following:

**CAD-Geometry (included in A+W CAD Services):**
Service provides the shape catalog, which is loaded once at when A+W iQuote is started.
Log in default Windows log directory: `C:\ProgramData\A+W\Log`
Ex. `CAD.GeometryService_2021-10-11.38616.0.awtrc`

**Commercial converter**
Service communicates with the documentservice (Backend) and provides the communication to Windows services or takes over the tasks that are not possible via the Backend. Activating CAD service, AWDesign or the fetching and provision of reports/attachments.
Log in default Windows log directory: `C:\ProgramData\A+W\Log`
Ex. `Commercial.ConverterService_2021-09-28.13000.0.awtrc`

**Web configurator**
Service is the main interface between Web browser and the Backend (documentservice). All communication calls run via the Web configurator.
Log in default Windows log directory: `C:\ProgramData\A+W\Log`
Ex. `Web.ConfiguratorService_2021-10-11.39272.0.awtrc`

**Commercial document**
The service (documentservice) takes over all tasks as "A+W Enterprise clone". Each call from the Web lands with the documentservice later on.
Log is in Unix in the log directory (`gp`)
Ex. `awsoa_documentservice_54138_1011`

In addition to the above-mentioned log, the documentservice also writes ftests if a calculation has been run through.
Test is on Unix in the ftest directory (`gft`)
Ex. `documentservice_54138.test`

### 22.4. Export of the Memrels sketches

With the DevOps item #101907 a possibility was created to export the Memrels sketches to `$REPTMP`. Some information from the Memrels is written to data objects and transferred to the ConverterService for sketch generation.

We have a crash with the call of the ConverterService at a customer's.
Following message content:
> Iceutilexeption: /usr/include/IceUtil/handle.h
> iceUtil:NullHandleException

The crash is probably caused by corrupt data in the data object to be transferred; that's why the hope is that the information from the Memrels will give us something with regard to the cause of the crash.

The export overwrites the existing files after each sketch generation.

The environment variable `IQUOTE_SKETCH_MEMREL_EXPORT` must be set to `ON`.

The exported Memrels are written to `REPTMP`. The environment variable `REPTMP` must therefore be maintained accordingly.

Export file name: `MEX_Maskenname.Userld` Example `MEX_KPOS.-1`
