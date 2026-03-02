---
description: "EN-UM-AW_iShape"
---


# A+W iShape Manual

---
## Editorial

### Revision overview of the documentation

| Date | Description |
| :--- | :--- |
| 08-2023 | Update of chapter XTREAM |
| 06-2022 | App release in version 2.0 |
| 03-2021 | Original version |

### Notes

This document is intended only for end users of A+W iShape.

The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

This document describes the full scope of A+W iShape.

### Copyrights

© 2024, A+W Software GmbH all rights reserved, also those for reprinting, the making of copies and translation.

The documentation may be copied, completely or in part, saved in an archiving system or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH's prior written approval.

### Trademarks

All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### Display conventions

Individual elements of the sentences are displayed in a special form. The meanings are:

- **Italics**: marks character strings describing the software elements, e.g. the *Buckets* dialog.
- **Bold**: marks character strings to be entered via keyboard, e.g.: **Enter 0**.
- **>**: shows the way to open a dialog, e.g. Display > Filler orders > Context menu - List > Order overview.
- **[]**: square brackets mark the buttons in the dialog, e. g. [OK] to save the data.
- **< >**: pointed brackets refer to keys or shortcuts on the keyboard, e. g. <F1> is used to open the online help.

### Contact

**A+W Software GmbH**
Siemensstr. 3
D-35463 Fernwald
Germany

Tel.: +49 641 96620 0
E-Mail: info@a-w.com
Web: http://www.a-w.com

## Contents

- **Overview (A)**
- **Tutorial (A-9)**
- **Documentation (A-12)**
- **Basics (A-13)**
  - Using the ruler (A-14)
    - Ruler - sizes (A-14)
    - Number of rulers (A-15)
    - Ruler - distance to the edge (A-16)
    - Ruler - placement (A-17)
    - Using the ruler as triangle (A-18)
    - Freeing up the rulers (A-19)
  - Requirements for pictures (A-20)
    - Picture properties (A-21)
    - Picture focus (A-22)
    - Picture background (A-23)
    - Picture contrast (A-24)
    - Picture lighting (A-25)
    - Picture quality (A-26)
  - Fastening (A-27)
    - Fastening material (A-28)
    - Set-up of the templates (A-30)
- **Sample pictures (A-31)**
- **The application (A-33)**
  - Display elements (A-34)
  - Operation (A-35)
  - App activation (A-36)
  - Gallery (A-37)
    - Non-processed images (A-39)
    - Processed images (A-40)
    - Delete images (A-43)
  - Process image (A-44)
  - Templates - confidence (A-46)
  - Taking a picture (A-48)
  - Pictures - import (A-49)
  - Contour display (A-50)
  - Contour - full image and zoom (A-51)
  - Settings (A-52)
    - Language (A-54)
    - Information (A-55)
    - Help (A-56)
    - Log files (A-57)
- **iShape files in the A+W CAD Designer (A-58)**
  - Open iShape file (A-59)
  - Process iShape file (A-60)
  - Tools for post-processing (A-60)
  - Smoothing (A-61)
  - Join several segments (A-62)
  - Resolve round corners (A-63)
  - Correcting curves: option 1 (A-65)
  - Correcting curves: option 2 (A-67)
  - Manual creation of the edges (A-68)
  - Visibility of the background image (A-70)
  - Adjustment of XTREAM (A-72)

## A+W iShape Overview

### Revision overview of the module

| Date | Description |
| :--- | :--- |
| 2023-08 | Update of chapter XTREAM |
| 2022-06 | App release in version 2.0 |
| 2021-03 | Original version |

This module provides information on the following subjects:
- Tutorial

## Tutorial

This section provides information on the following subjects:
- Documentation
- Basics
- Sample pictures
- The application
- iShape files in the A+W CAD Designer

### Documentation

A+W iShape offers a simple, flexible solution for generating digital data from shape templates (non-rectangular lites). The digitalization of lites is done with a camera.

The template is fitted with L-shaped reference objects and then photographed with a high-end smartphone camera. The reference objects, high-quality precision metal pieces, are laid on or fastened to the template. They serve to correct any distortions when photographing. The objects also have a QR code, which enables automatic detection of the objects and thus makes additional configuration unnecessary.

The special feature: in contrast to older solutions is that no calibration of the camera is required! A+W iShape works with any good mobile phone camera. After the photo has been taken and the picture processed, the shape detected can be checked and forwarded directly from the smartphone.

The further processing of the files is done in A+W CAD Designer (Shapes): machine data or DXF files can be generated here. The entire recording process takes just a few minutes.

This description of the A+W iShape will show you how you can use the module and to what you need to pay attention when working with the camera.

#### Requirements

The A+W iShape module assumes use (installation) of the current A+W CAD Designer (Shapes) version. Knowledge of A+W CAD Designer (Shapes) is also useful. A+W iShape should already be installed and configured.

## Basics

The development of A+W iShape is based on the peculiarity in production: For manufacturing of a non-rectangular lite (shape, free shape), glass processors frequently receive a hand drawing or a wood, chipboard, or cardboard template from their customer. The shape of these lites can be detected and digitalized with A+W iShape.

The series of points (contour) generated is then opened in A+W CAD Designer (Shapes) and can be corrected with the tools present in A+W CAD Designer (Shapes). Thus, the final contour is generated in the end according to the user's wishes. For example, corners can be rounded off here or the contour extended by specified distances on particular edges. All of this builds on familiar A+W CAD Designer (Shapes) functionalities so that reference is made here to the appropriate documentation. Then, these files can be used in production on CNC machines.

> **Additional information**
> The following chapters describe using some pictures what requirements the pictures taken have to fulfill in order to digitalize the shapes as easily and quickly as possible.
> - "Using the ruler" on page A-14
> - "Requirements for pictures" on page A-20
> - "Fastening" on page A-27
> - "Sample pictures" on page A-31

### Using the ruler

In order to detect the shape contours, various rulers are used in A+W iShape. These are angled rulers with a QR code. This QR code is also called the DMC (Data Matrix Code).

The description and correct use of the rulers follow here:
- "Ruler - sizes"
- "Number of rulers"
- "Ruler - distance to the edge"
- "Ruler - placement"
- "Using the ruler as triangle"
- "Freeing up the rulers"

#### Ruler - sizes

There are three different ruler sizes for A+W iShape:
- Size L (DIN A3)
- Size M (DIN A4)
- Size S (DIN A5)

The rulers can be combined in any way. However, it has to be possible to clearly detect the DMC. To be noted here, among other things, is that the larger the picture, the further the distance from the camera and thus the QR codes on smaller rulers would be difficult to detect.

To be noted also is that the QR code of the small rulers is difficult to see on large shapes. That's why the size S rulers should be used on small shapes.

#### Number of rulers

The number of rulers used depends on the shape size. The larger the shape, the more important it is to place enough rulers on the shape. That is, six rulers are enough for a large shape, while one ruler is never sufficient. Three rulers are also seldom enough, except for very small shapes.

The number of rulers depends on the number of corners on the shape.

*Examples:*

*Fig. A-1: Examples of the different numbers of rulers in pictures*
- *A) Insufficient number of rulers*
- *B) Sufficient number of rulers*

#### Ruler - distance to the edge

Place the ruler (L-shaped tool) on the shape approx. 0.5 centimeter (1/4 inch) from the edge.

*Examples:*

*Fig. A-2: Sufficient ruler distance to edges*

*Fig. A-3: Insufficient ruler distances to edges*
- *A) Too far from the edge*
- *B) Too close to the edge*

#### Ruler - placement

The rulers are placed along the contour. All corners of the template must also be covered with the rulers. Together, the outermost reference points of the rulers form the convex envelope. During ruler placement, pay attention that it is maximized.

*Examples:*

*Fig. A-4: Appropriate ruler positioning to edges and corners*
- *A) Correct positioning of the rulers*
- *B) With convex envelope*

*Fig. A-5: Insufficient or incorrect positioning of the rulers on the contours and corners*

#### Using the ruler as triangle

The edges of the ruler form a triangle whose whole surface has to be within the shape. The content of the stretched triangle is used as orientation for which color the shape is. The rulers should be laid so that no labels, stickers or anything else is within this triangle. This could distort the coloration.

*Examples:*

*Fig. A-6: Use of the ruler as triangle*
- *A) Entire triangle inside the shape*
- *B) The circumscribed triangle is inside the shape*

*Fig. A-7: Impermissible use of the ruler as triangle*
- *A) Parts of the circumscribing triangle are outside the shape*
- *B) Parts of the triangle are mixing with the labeling*

#### Freeing up the rulers

All rulers are placed so that the sides of the rulers neither interlock nor overlap one another.

*Examples:*

*Fig. A-8: Correct positioning of the rulers with respect to one another*

*Fig. A-9: Incorrect ruler positioning with respect to one another*
- *A) Interlocking ruler placement*
- *B) Overlapping ruler placement*

### Requirements for pictures

In order to transfer the pictures to A+W iShape, the following points have to be considered:
- "Picture properties"
- "Picture focus"
- "Picture background"
- "Picture contrast"
- "Picture lighting"
- "Picture quality"

#### Picture properties

In the picture, the whole shape and only a bit of the background should be clearly visible. Avoid photographing too much background or cutting off parts of the shape. In no case may the reference points or the data matrix code on the ruler be cut off.

*Examples:*

*Fig. A-10: The right relationship between the template and the background in the picture*

*Fig. A-11: Picture properties: relationship between the template and the background*
- *A) Shape contour is cut off*
- *B) Picture was not taken correctly: DMC is not visible*

#### Picture focus

In order to fully exploit the camera's focus, a simple, flat object can be positioned in the middle of the template.

*Example:*

*Fig. A-12: Placement of an object in the middle of the template for better focus*
- *A) Sufficient focus*
- *B) Significantly better focus*

#### Picture background

The picture should be taken with as homogeneous a background as possible.

*Examples:*

*Fig. A-13: The light, e.g. gray, background is best for a picture*

*Fig. A-14: Picture properties: examples of unsuitable picture backgrounds*
- *A) "Busy" background*
- *B) Carpet - background*

#### Picture contrast

There should be enough contrast between the shape and the background. Avoid light shapes against light backgrounds. With light shapes, a dark background such as black cloth or felt is recommended. This ensures optimal contrast and prevents unwanted shadows on the shape.

*Examples:*

*Fig. A-15: Examples of different levels of contrast in pictures*
- *A) Good contrast between the template and the background*
- *B) Poor contrast between the template and the background*

#### Picture lighting

The picture should be neither too bright nor too dark. Avoid shadows or reflections on the picture.

*Examples:*

*Fig. A-16: Examples of the different lighting levels in pictures*
- *A) The picture is too bright*
- *B) The picture is not bright enough*

*Fig. A-17: Examples of the different shadows in pictures*
- *A) The picture has a shadow*
- *B) The picture has reflections*

#### Picture quality

Try not to wobble when you're taking the picture and wait (if necessary) until the camera has focused. If the picture is blurry, the data matrix code can't be read.

*Examples:*

*Fig. A-18: Examples of poor picture quality*
- *A) The picture is blurred*
- *B) The DMC code is not clearly visible*

### Fastening

In order to be able to take pictures of the required templates and the rulers on them, both the templates and the rulers must often be fastened.

The following chapters describe what you must pay attention to here:
- "Fastening material"
- "Set-up of the templates"

#### Fastening material

To fasten the rulers to the templates, you can use pins. Please note that these must be pins with flat heads. With flat-headed pins, you must also pay attention to the selection of the color for the pins: white or very light pins can be detected as marking points for the rulers and thus possibly distort the confidence value. If you are using pins, holes must be drilled for these in the rulers. Please make sure to put the holes only between the white points.

*Example:*

*Fig. A-19: Example of poor pin placement*
- *A) Pins are stuck over the marking points*

Furthermore, neither rulers nor template edges may be glued over. However, tape strips can be used as an alternative fastening method if they stick on both sides and are fastened on the back of the rulers or templates.

*Example:*

*Fig. A-20: Example of poor template fastening*
- *A) The tape strips are covering the marking points and protrude over the edge*

In the following picture, pins and double-sided tape strips are used optimally on the back of the template:

*Fig. A-21: Example of good template fastening*

#### Set-up of the templates

To photograph the templates properly, they must generally be well-placed or set up. A wall can offer good possibilities for placing templates. You can lean the templates on the wall, set up a kind of set-up edge or use various tools for the set-up, e.g., screws. The set-up of the template is easier if the surface is slightly tilted.

*Examples:*

*Fig. A-22: Examples of good template set-up*
- *A) The templates were set up on the wall and fastened with screws of dowels*

## Sample pictures

There are some sample pictures below. These sample pictures include various shapes of templates and possible L placements that provide very good results.

*Fig. A-23: Sample pictures*

## The application

> Both the app display and operation of the A+W iShape app were reworked in Version 2.0. This documentation describes the new features. In principle, the application can be operated intuitively. Work with the A+W iShape app assumes general knowledge of smartphones.

Nevertheless, the individual operating and display elements will be explained in the following sections:
- "Display elements"
- "Operation"
- "App activation"
- "Gallery"
- "Processed images"

**App alignment**
During operation, the app works permanently in portrait format. Only in the zoom function can the display be turned to landscape format.
- "Contour - full image and zoom"

### Display elements

The following table describes all icons that are used throughout the application:

| Icon | Name | Meaning |
| :--- | :--- | :--- |
| 🖼️ | Gallery | This icon indicates the gallery view. |
| 📷 | Camera | Use this icon to start photographing with the camera. |
| 📂 | Image import | Use this icon to start the image release from the camera view. |
| ⚡ | Camera flash | Use this icon to switch the camera flash on/off. |
| ⚙️ | Settings | Use the gear icon to access the app settings. |
| < | Back | Use this icon to return to the previous page. |
| ☑️ | Checkbox marking | Using the checkbox icon, you select one or several images or files and can take further action, e.g. export or delete these files. |
| 📤 | Release for... | Using this icon, you can export images or files. |
| 🗑️ | Trash can | Using this icon, you can delete the marked images. |
| 🔍+ | Zoom in | Using this icon, you can zoom in on the image view. |
| 🔍- | Zoom out | Using this icon, you can zoom out of the image view. |

**Icon explanation:**
Depending on the context, these icons may look as follows:
- **blue**: active = touching triggers a corresponding action.
- **gray**: inactive = the action is currently not available.

### Operation

This section describes the sequence of steps for working with the A+W iShape app. This description assumes that you have already acquired the app and installed it on a smartphone.

**The app provides this flow:**
1. Prepare the template that you want to process with the app.
2. Place the rulers required for detection on the template. Heed the requirements described in the following section: "Using the ruler".
3. Prepare the template with the rulers for photography: "Requirements for pictures".
4. Photograph the prepared template or perform steps 5-6.
5. Start the app.
6. Via the app, select the photography option ([Camera] icon): "Taking a picture".
7. Use the app gallery for the overview and processing of the images: "Gallery".
8. Let the app process the images: "Process image".
9. Check the confidence of the template detected. You can repeat the foregoing steps until you achieve the result desired: "Templates - confidence".
10. Release the processed image file in order to process it in A+W CAD Designer (Shapes): "Contour display" and "iShape files in the A+W CAD Designer".
11. Work through all templates in this manner.
12. Close the app.

### App activation

*iShape app*
When you start the new app version for the first time, you will see an activation request. When you purchase the app, you will receive a QR code that you have to scan for activation. After successful activation, you can use the application.

*[Image: App page with activation request. Shows a screen titled "Activation" with a message "Scan your license QR code" and a "[Scan]" button.]*

> **Additional information**
> - "Gallery"
> - "Processed images"

### Gallery

*iShape-App > Gallery*

*[Image: App gallery screen showing two tabs "Not processed" and "Processed", with an empty state message "No templates available".]*

The app starts with a gallery that is divided into the following areas:
- Not processed
- Processed.

At first, both areas are empty. To process the images in the app, they must be made available in the app. You can photograph the templates to be processed with the smartphone or upload pictures you have already taken via the smartphone import function. These possibilities are described in the following sections:
- "Taking a picture"
- "Pictures - import"

The new images upload are listed on the Not processed tab:
- "Non-processed images"

By simply touching the existing image, you can continue processing it:
- "Contour display"

Processed images are listed in the appropriate area. By touching [Processed], you change to the appropriate view:
- "Processed images"

#### Non-processed images

*iShape app > Gallery > "Not processed" area*

*[Image: App overview "Not processed" showing a list of unprocessed images with filenames and timestamps.]*

In the *Not processed* area, the images are listed that are now available for processing. By simply touching the desired image, you can forward it for processing. You will be taken to the next page: "Process image".

By touching and holding, you mark the desired image and thus have the opportunity to delete the images: "Delete images".

#### Processed images

*iShape app > Gallery > "Processed" area*

*[Image: "Processed" app page showing an empty state, "No templates available".]*

In the *Processed* area, you get an overview of all images that have been processed recently. This view appears if you start the app for the first time or if you have already deleted the last images processed.

*[Image: App page with processed images. Shows a list of processed items, each with a thumbnail, filename, timestamp, number of rulers detected (e.g., 5/5), and a circular confidence score (e.g., 90%, 70%, 30%).]*

If you have processed the images, the appropriate overview appears in the *Processed* area.
In the new app version, for each processed image you get the confidence reached via the template detection, which is depicted using a colored ring chart.

The meaning of the ring charts is as follows:

| Icon | Name | Meaning |
| :--- | :--- | :--- |
| 🟢 | Green ring | This icon indicates the shape detection in the 80 to 100% range. The percentage in the middle of the icon specifies the confidence. |
| 🟡 | Yellow ring | This icon indicates the shape detection in the 60 to 80% range. The percentage in the middle of the icon specifies the confidence. |
| 🔴 | Red ring | This icon indicates the shape detection in the 10 to 60% range. The percentage in the middle of the icon specifies the confidence. |
| ❗️ | Red ring with exclamation point | This icon indicates that the shape detection was less than 10% or that no shape could be detected. |

By touching and holding the desired file/s, you mark it/them and thus have the opportunity to delete the file/s: "Delete images".

> **Additional information**
> - "Gallery"
> - "Taking a picture"
> - "Pictures - import"

#### Delete images

*iShape-App > Gallery > Select image/s*

*[Image: App page for deleting images, showing a selection mode with checkboxes next to each image and a trash can icon at the top.]*

You can remove the listed images at any time from both areas of the gallery. For deletion, you can swipe the existing file to the side. This removes precisely one image from the app.

To delete several images at one time, touch an image and hold it briefly with your finger. Checkboxes are displayed for the links to images. Activate these checkboxes for all images that should be deleted. Then use the trash can icon. This deletes all marked images from the app.

Touch the [x] icon to close the current dialog and return to the app.

> **Deleting images**
> If you delete images in the app, they are also deleted in the file explorer on your smartphone!

### Process image

*iShape-App > Gallery > Select image*

*[Image: App page for image processing, showing a selected image thumbnail, its filename and timestamp, and a [Process] button.]*

The selection of an image in the gallery takes you to another page where you have the following possibilities:
- To process the selected image ([Process] button)
- To return to the gallery ([<] icon)
- To release the selected image ([Release for] icon).

#### Ruler - selection

*iShape-App > Gallery > Select image > Process*

*[Image: App page for ruler selection, showing an image and a "Cancel" and "Confirm" button over a scrollable list of ruler counts (e.g., 3 Ls, 4 Ls, 5 Ls).]*

To process the template as quickly as possible, the app requires specification of the number of rulers. Swipe up or down with your finger to make the appropriate specification. Confirm your selection.
Alternatively, you can Cancel the processing and return to the previous screen.
After confirming the number of rulers, the current image is processed in the A+W iShape app.

> **Additional information**
> - "Templates - confidence"
> - "Process image"

### Templates - confidence

*iShape-App > Processed templates > Notes*

*[Image: App page with confidence notes. It displays the processed image, file details, a confidence score (70%), ruler count (5/5), a "Show Contour" toggle, and a "Hint" box with suggestions like "Move L rulers closer to contour..."]*

You can get a report about the possible cause for why the template detection did not work from the corresponding note. This information is displayed directly after image processing or if you touch alternatively on the already-processed image in the gallery.

In the associated detail view, you can get the following information:
- **The image display.** By touching the zoom in icon, you can enlarge the image; by double-tapping it, you can zoom in on the image.
- **The file name and date** of the last processing.
- **Confidence value** as ring chart with the percentage.
- **Specification of the rulers** (e.g. L 6/6 means that 6 of 6 rulers were detected).
- **Contour switch** (green line on the template) for switching on and off
- **List with notes.** For additional notes, if there are any, scroll the image up.
- You can **release the image** with the [Export] icon.

The following notes are possible here:
- One or several L reference objects were not detected. Take a picture with all L reference objects in focus.
- The template is not centered vertically. Move the camera down.
- The template is not centered vertically. Move the camera up.
- The template is not centered horizontally. Move the camera to the right.
- The template is not centered horizontally. Move the camera to the left.
- Move the camera further away from the template.
- Take a picture with a centered perspective.
- Use more L reference objects.
- Move the L reference objects closer to the contour or cover more template area with the L reference objects.
- Try a more symmetrical arrangement of the L reference objects around the middle of the image.

To exit or return to the previous screen, please touch [<].

### Taking a picture

*iShape app > Camera*

*[Image: App camera screen showing the live view of a template with rulers. At the bottom are icons for image import, the shutter button, and camera flash.]*

Use the [Camera] icon to take the picture. Position the camera correctly. Heed the requirements for pictures and the correct use of the rulers.

Tapping the take picture button takes the picture. As soon as the camera has taken the picture, you are taken to the next page. You are only taken to the next page if the *Several Images* setting is deactivated. Otherwise, you can take several pictures one after another without moving on. This is the default setting in the current app version.

With the [Flash] icon you can turn on the optional camera flash if it is too dark. Note also that the flash can cause reflections.

With the [Open] icon, you can import an existing image into the app.

Use the [<] icon to return to the previous page.

### Pictures - import

*iShape-App > Picture Import*

*[Image: Smartphone's file explorer interface for importing a picture, showing a gallery of recent photos.]*

With Picture - Import, you can import existing pictures into the A+W iShape app. Here, the default file explorer on your smartphone opens. At the top of the screen, you have your smartphone's standard functions, including storage location selection, search, change view. Generally you can also control the display sorting. In the example, the last pictures taken are displayed.

By touching the picture, you select it in order to import it into the A+W iShape app. If you can select multiple photos on your smartphone, you should know that such a multiple selection is not supported in A+W iShape; only one photo is imported.

After the selection, you can process the image directly: "Process image".

### Contour display

*iShape app > Process image > Contour*

*[Image: App page showing a processed image with the detected contour highlighted as a bright green line around the shape.]*

If you have set the *Contour on* option in the settings, the shape processed is surrounded by an illuminated line. Here you can check the results of the processing visually.

You can also show or hide this option at any time: "Taking a picture".

Further along, you can enlarge or zoom in on the image if necessary: "Contour - full image and zoom".

#### Contour - full image and zoom

*iShape app > Process image > Contour*

In this view, you have the opportunity to display the image in full image mode. For this, touch the [Large view/on] icon. To switch off full image mode, touch the [Large view/off] icon.

In the image processing and in full image mode, you can zoom in on the images. Touch the picture twice or touch the display with two fingers and spread your fingers to enlarge the picture area. This is how to enlarge the image or the image section as you wish. In full image mode, the smartphone can also be used in landscape format.

To reduce the picture, draw your fingers back together or double-tap again.

### Settings

*iShape-App > Settings*

*[Image: App settings page showing various options like "Number of L rulers", "Display camera preview section", and toggles for "Several Pictures", "Show Contour", "Show Processing Feedback".]*

Use the gear icon to access the page with the settings. Here you can make the following settings:

- **Number of L reference objects**: Default setting for the number of rulers, which is suggested before picture processing. This value can be changed as necessary before each image processing. The setting only influences the duration of the processing of the picture taken.
- **Preview display in the camera**: Preview display in the camera. Here you specify the percentage to which the preview is limited. By default, the value is 70%.
- **Continuous pictures: on/off**: Switches on continuous picture-taking. If the Continuous picture mode is activated, you can take several pictures in sequence without having to go to the next page. All pictures taken are saved in the gallery and can be edited after the fact. Drag the slider to the right if you would like to activate this option. By default, continuous picture mode is switched on. This setting does not apply for the image import.
- **Contour on/off**: Default setting for the contour display. By default, the slider is active and the contour is displayed. Drag the slider to the right if the contour should no longer be displayed directly.
- **Processing messages on/off**: This setting deactivates any feedback except for the number of rulers. No confidence value and no notes are displayed. This setting should only be deactivated in particular cases.

Via the settings, you can access other pages:
- "Language"
- "Information"
- "Help"
- "Log files"

> **Changes to the settings**
> The changed settings are active right away in the app. That is, if you change the language, e.g., the app switches to the appropriate language immediately after saving.

#### Language

*iShape-App > Settings > Language*

*[Image: App language settings page, showing a list of available languages (Czech, German, English, etc.) with a checkmark next to the selected one.]*

Use this page to change the app language. By default, the language is selected that you have specified on your smartphone.

A+W iShape exists in the following languages (sorted by language abbreviation):
- Czech (CS)
- German (DE)
- English (EN)
- Spanish (ES)
- French (FR)
- Italian (IT)
- Dutch (NL)
- Polish (PL)
- Portuguese (PT)

The [Save] button is activated when the language is changed and it must be pressed to save the changes made.

#### Information

*iShape-App > Settings > Information*

*[Image: App information page, displaying Device Identifier, Device Name, App Version, and Digitizing Version.]*

Via this page, you can view information about the app installation. The following information is displayed:
- Device detection for your smartphone
- Device name of the smartphone
- App version - version number of the installed app
- Digitizing version - version number of the associated service

Use the [<] icon to return to the settings.

#### Help

*iShape-App > Settings > Help*

*[Image: App help page, showing the A+W iShape logo, contact email, and copyright information.]*

On this page, you can make contact with A+W Software GmbH, call up the company's official home page, and the copyright information.

Use the [<] icon to return to the settings.

#### Log files

*iShape-App > Settings > Log files*

*[Image: App log files page, showing a list of text files (e.g., 20220704.txt) with checkboxes next to them and a share/release icon.]*

On this page, you can forward the log files created, that is, send them via e-mail to the responsible A+W Software GmbH employee.

Select the desired log file/s by activating the checkbox and touching the [Release for] icon.

Use the [<] icon to return to the settings.

## iShape files in the A+W CAD Designer

Files digitalized in A+W iShape can be processed further in A+W CAD Designer (Shapes).

A few basic steps are described below:
- "Open iShape file"
- "Process iShape file"
- "Smoothing"
- "Manual creation of the edges"
- "Visibility of the background image"
- "Adjustment of XTREAM"

### Open iShape file

*A+W CAD Designer (Shapes) > Open File*

A file with the file extension `.ishape` can be opened in A+W CAD Designer (Shapes) either via the menu or directly with the marked icon.

*[Image: A+W CAD Designer (Shapes) application window.]*

*[Image: Windows 'Open' dialog showing the file type dropdown, with 'File (*.ISHAPE)' selected.]*

Then the standard Windows Open dialog opens. To be able to open the .ISHAPE, open the field at the bottom right of the dialog and select File (*.ISHAPE). Then the ISHAPE file can be opened.

### Process iShape file

#### Tools for post-processing

To post-process the A+W iShape shape, you will need the following tools in A+W CAD Designer (Shapes):

| Icon | Name | Description |
| :--- | :--- | :--- |
| ↔️ | JOIN | Join two segments (select point between segments). |
| ✂️ | SPLIT | Divide a segment into two segments (select segment, set point). |
| 🔄 | RNDEDGE | Round a segment (select segment between segments). |
| 📐 | DESIGNC | Shift a segment to the inside/outside with adjustment of the corners. |
| ↕️ | MSEGORTH | Shift a point vertically to the segment (can be adjusted with the + and - keys). |
| ↗️ | MSEGTANG | Shift a point tangentially to the segment (can be adjusted with the + and - keys). |
| 📏 | DIGLINE | Create the best line from digitalized points. |
| ⌒ | DIGARC | Create the best curve from digitalized points. |

> **A+W CAD Designer (Shapes) Configuration**
> If not all tools are included in the interface in the A+W CAD Designer (Shapes), they have to be added in the sn.ini.

### Smoothing

*A+W CAD Designer (Shapes) > Open File (opened iShape file)*

*[Image: An opened iShape file in A+W CAD Designer, showing the raw, un-smoothed contour over the background photo of the template.]*

To process the iShape file in A+W CAD Designer (Shapes), a few steps are required. The procedure and the tools required for this are explained with the smoothing of this shape (see picture).
- "Join several segments"
- "Resolve round corners"
- "Correcting curves: option 1"
- "Correcting curves: option 2"
- "Manual creation of the edges"

### Join several segments

*A+W CAD Designer (Shapes)*

With the **JOIN** tool, you select a point (marked in red here) whose adjacent segments should be joined. Under some circumstances, this step has to be repeated several times.

*[Image: A contour in CAD Designer with many small segments. One point is highlighted in red, ready to be joined.]*

Then the result might look like this:

*[Image: The same contour after using the JOIN tool, showing fewer, longer segments and a smoother overall shape.]*

### Resolve round corners

*A+W CAD Designer (Shapes)*

To resolve the rounding of a corner, select the **RNDEDGE** tool and include the segment for the corner.

*[Image: A rounded corner in CAD Designer is selected, with the RNDEDGE tool active and showing a radius value.]*

If you now set the value to 0, the result as follows:

*[Image: The same corner, now sharp (90 degrees) after setting the radius to 0.]*

The whole thing also works the other way around; if you would like to enlarge the rounding, enter a larger value.

### Correcting curves: option 1

In this picture, the contour is not precisely along the edge of the shape. This can be corrected in A+W CAD Designer (Shapes). Previously, the segment marked in red is divided into two segments with the **SPLIT** tool.

*[Image: A close-up of a curve in CAD Designer where the detected red contour line deviates from the actual edge of the shape in the background image.]*

The tool **DESIGNC** shifts the marked segment parallel and adjusts the surrounding segments. Depending on whether you enter a positive or negative value, the segment shifts to the outside or inside. The application of the tool leaves the shape looking as follows:

*[Image: The same curve after using the DESIGNC tool. The red contour line now perfectly matches the edge of the shape.]*

If you select a segment after the processing, the original course of the edge is displayed in light gray.

### Correcting curves: option 2

The tools **MSEGORTH** and **MSEGTANG** offer another possibility for editing curves. Thus, the points can be shifted either vertically or tangentially to the original segment. If you have specified a value, the shifting can be adjusted with the + and - keys. Thus, you can shift the point along the orthogonals or tangents in both directions. On the value window, you can specify under 1, 2 and c whether the transitions to the corresponding points should be smooth. Here it must be noted that minimum and maximum two of the three options can be allowed.

*[Image: A curve being edited with the MSEGORTH/MSEGTANG tools, showing handles and value inputs to adjust the point.]*

If you edit the curve with these tools, the result might look like this:

*[Image: The result of the curve correction, showing the adjusted contour line. The original curve is shown faintly in the background for comparison.]*

Here too, you can display the original course of the curve if you select one of the segments after the processing.

### Manual creation of the edges

It is also possible to create the edges manually. For this, you need the tools **DIGLINE** and **DIGARC**. These create the best line or the best arc along the marked points.

For this, you mark the start and end point along which the best line is generated in this example. The direction when marking the points has to be noted. It corresponds to the direction in which the points were created.

*[Image: A section of points in CAD Designer before manual edge creation.]*

After application of the tool, the edge looks like this:

*[Image: The same section of points with a new, straight edge created using the DIGLINE tool.]*

Accordingly, the **DIGARC** tool has to be used for arcs.

This method has the advantage that it gives the creator of the shape more control and therefore, greater precision can be achieved. Once you have begun with this method, you should continue across the rest of the shape since inconsistent application can cause poor results.

### Visibility of the background image

*A+W CAD Designer (Shapes) > View > Preferences > Background Image > Opacity*

With this menu path, the visibility of the background image can be set.

*[Image: A screenshot showing the menu path to adjust the background image opacity, with options from 20% to 100%.]*

The menu entries can also be added to the context menu for quicker access. For this, the MenuID and AdditionalTextForXXXXX entries were added to the PopUp section of the SN.ini.

Example: The menu entries 40% opacity and 100% opacity can be displayed with the following configuration:

```ini
[PopUp]
MenuID = 32925
MenuID = 32928
AdditionalTextFor32925 = Opacity
AdditionalTextFor32928 = Opacity
```

The menu identifiers are 32924 - 32928 for the entries 20% - 100% in 20% steps. The additional text can be selected as you wish.

To activate the menu element, the following requirements have to be fulfilled:
- A background image is displayed
- You are in the Point or Geometry view

A new parameter was also added to the SN.INI:

```ini
[Digi]
BackgroundImageOpacity = 0.2
Possible values: 0.0 - 1.0
```
This value is used when A+W CAD Designer (Shapes) is started. By using the menu element to make changes, only the currently running instance of the value is adjusted.

*[Image: The right-click context menu in CAD Designer, showing custom "Opacity" options added.]*

### Adjustment of XTREAM

> **Adjustments in sn.ini**
> The settings in the sn.ini configuration file are only for your information and should only be changed by the system administrator.

**XTREAM** is the algorithm that is used for edge smoothing.

Standard process **XTREAM** is particularly suitable for smooth shapes. This method has now been upgraded with improved corner detection. In addition, the remaining area of the shape is now also smoothed by **XTREAM** during manual regression, so that the user can now also smooth partial areas manually.

The **Shape XTREAM** method has advantages over the standard corner detection method. This method prefers the generation of straight lines instead of circular arcs in some places. Another difference arises when additional areas of the shape are smoothed manually by inserting regression segments. In the standard **XTREAM** method, a simplified method is applied to the remaining area, so that in many cases the user must manually approximate the entire shape by regression segments for optimal results.

Both methods can be manipulated by different parameters in the SN.INI file.

Below is an excerpt from the sn.ini with the important switches for **XTREAM**:

```ini
[XTREAM]
AccuracyForToolAngZero = 0.1 mm
CAPTURERADIUS = 1.125
CloseOpenShapes = 1
DEFAULTBORDER = 10.
DigiWheelForCheckpointsRadius = 6.35
DigiWheelRadius = 6.35
MAXCORNERANGLE = 25.
MAXRADIUS = 10000.
MINDIGIDIST = 0.75
MINIINTERIORRADIUS = 125.
NORMACCURACY = 1.25
SegmentInfo = 0
ForceTangentAngleZero = 0
ShowPointsForSelection = 1
LineLimit = 0.5
PointsPerInterval = -1
IntervalLength = -1
IShapeDoModel = 0
FINDCORNERS = 1
```

- Setting the `CloseOpenShapes` parameter to 1 forces the contour found to be closed. This is important for the later import of the SN/DXF file into A+W Business/A+W Enterprise.
- By changing the parameter `NORMACCURACY` you can specify the precision of the smoothing, for example. A value around 1 has proven to be a good setting.
- Setting the parameter `IShapeDoModel` enables the **Shape XTREAM** method.
