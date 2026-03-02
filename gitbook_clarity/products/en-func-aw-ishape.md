---
description: "EN FUNC A+W iShape"
---



# EN FUNC A+W iShape

     Functional Description


A+W iShape




                              english
1. Content
1.       Content                                             3
2.       Notes on this Document                              4
  2.1.   Trademarks                                          4
  2.2.   Copyrights                                          4
  2.3.   Disclaimer of liability                             4
3.       Performance Description                             5
  3.1.   Data                                                5
  3.2.   Description                                         5
  3.3.   Requirements                                        5
  3.4.   List of functions                                   6
  3.5.   License modules                                     7
  3.6.   Limitations                                         7
  3.7.   Notes                                               7
4.       Contact Address                                     8




A+W Software GmbH                  EN-FUNC-A+W iShape.docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license. The content of the documentation serves only as
information and can be changed without prior notice at any time. The text and illustrations were
compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH
assumes no liability for errors or imprecise statements unless these can be traced back to
intentional or negligent actions.


2.1. Trademarks
All hardware and software names mentioned in this documentation might also be registered
trademarks or other property rights of third parties. The property rights of third parties must be
observed.


2.2. Copyrights
© 2021, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation may be copied, completely or in part, saved in
an archiving system, or transferred in any other form only in accordance with our license
agreement. Transmission of the documentation is not allowed, neither electronically, nor
mechanically, nor by recording or in any other way, without the written prior approval of A+W
Software GmbH.


2.3. Disclaimer of liability
A+W Software GmbH does not assume any liability for data errors resulting from the basics of the
standard functions provided by Microsoft, Unix or other software and hardware suppliers.
A+W Software GmbH reserves the right to change software data, structure, and interfaces as part
of program expansions without prior announcement. All amendments, extensions, database
queries, reports, analyses, and interface extensions which have been individually created for our
customers and/or machine and software partners as well as all related costs and expenses are to
be borne by the customer (customers, machine and software partners). This includes also any
necessary long-term costs and efforts for the expansion and adjustment of subsequent program
versions. This is necessary to make sure that the commissioned amendments/extensions which
have been made or developed for a version will work flawlessly and can be used in the successor
version.




A+W Software GmbH                      EN-FUNC-A+W iShape.docx                                       4
3. Performance Description
3.1. Data
 Product                A+W CAD Designer (Shapes)
 Module number 264001
 Module                 A+W iShape
 Brief                  Digitization of shaped sheets using a mobile telephone with
 description            high-end camera (iPhone >= iPhone 8, Huawai > P20)
 Available              Previous version available as of approx. end of March 2021,
                        restricted group of customers sought (after consultation).
                        Complete availability after completion of the pre-release
                        phase with selected customers. Prerequisite A+W SN
                        Version 6.4 or later


3.2. Description
The A+W iShape module is an add-on for A+W CAD Designer (Shapes). It enables the digitization
of shaped sheets (not rectangular sheets) using a camera. Primarily, as high-resolution camera as
possible on a mobile telephones should be used.
An APP (Android and IoS) is made available for the mobile phones, which in addition to the pure
recording of the shapes by the camera already does an initial quality check during the recording.
Alternatively, the picture can be created with a high-resolution camera and made available for
further processing in a special directory.
For calibration of the camera (balancing out of distortions), L-shaped rulers with precisely defined
points are used. The reference objects must be printed on suitable material or made available in
the best possible precision (< 1/10 mm). The scope of delivery includes an appropriate .pdf file.
The rulers can be purchased separately.
In the course of the examinations in the prototype status, other reference objects were also
tested. It emerged, however, the only the use of the L-shaped reference objects provides
sufficiently good results. Another advantage of these objects is that they are on the level of the
shaped sheets to be digitalized. Thus, the precision that can be achieved does not depend on the
thickness of the shape, which is a big advantage in practice. For operation of A+W iShape,
therefore, an available set of L reference objects is assumed.


3.3. Requirements
A+W iShape is an add-on for the A+W CAD Designer (Shapes). Accordingly, a current version of
the A+W CAD Designer (Shapes) must be available.
In addition, precisely printed L-shaped rulers are required, which must either be generated based
on the included .pdf file or purchased separately.



A+W Software GmbH                      EN-FUNC-A+W iShape.docx                                       5
A suitable mobile telephone must be available for the necessary camera. Currently tested were:
    •   iPhone 7, 8, 11, 12 and SE
    •   Huawai P20
The appropriate APP must be loaded on the mobile phone. The evaluation processes of the A+W
iShape are coupled via a cloud access. The A+W iShape cloud services must be licensed
appropriately for this.


3.4. List of functions




Several reference objects are placed on the contour to be digitalized. The contour is then
recorded with a camera together with these objects. The objects each have a QR code in the
corner, which ensures unique assignment. The familiar geometry of the reference object enables
the automatic calibration (equalization) of the recording, whereby the exterior contour is
transformed into a series of points along the contour.
In the first variant, the software tries to detect the existing exterior contour automatically. In the
later solution, it will also be possible to detect inner contours. For this, an area of the contours
will be selected later that belongs to the contour to be recorded. For this task, the APP must be
expanded accordingly on the mobile telephone.
The generated series of points can then be called up in the A+W CAD Designer (Shapes) via the
digitization tool. In the view that appears next, the point cloud can be seen against the
background of a mapping of the measured and equalized contour. Here, corrections of the data
are possible with the help of the tools in the A+W CAD Designer (Shapes). Thus, the final contour
is generated in the end according to the user's wishes. For example, corners can be rounded off
here or the contour extended by specified distances on particular edges. All of this builds on
familiar functionalities of the A+W CAD Designer (Shapes) so that reference is made here to the
appropriate documentation.
The reference objects are currently available in three sizes and two orientations:
    •   Size L (DIN A3)
    •   Size M (DIN A4)
    •   Size S (DIN A5)
A set of these objects, which can be ordered in addition to A+W iShape, consists of 9 objects:
three of each size, whereby two normal and one mirrored L is provided in each size.




A+W Software GmbH                       EN-FUNC-A+W iShape.docx                                          6
3.5. License modules
The list of required components emerges from all of this:
-       A+W CAD Designer
-       A+W iShape additional module for the A+W CAD Designer
-       A+W CloudService and mobile phone APP for providing services for the transformation
-       One set of reference objects (9-piece)


3.6. Limitations
An essential property of the solution is the precision that can be achieved and also the maximum
size of the shape sheets to be digitized.
The precision is influenced by several factors:
    1. The reference background must be printed and measured as precisely as possible. The
       distance of the circles and the diameter of the individual circles must be known precisely
       to less than 1/10 mm. The circles must all have the same diameter. As reference, a .pdf
       document is made available, which must be printed and measured in the desired size with
       the appropriate precision. On request, A+W will provide a set of these reference objects,
       which consists of 9 individual pieces; see above. According to the instructions (see
       documentation), the objects are placed as close to the edge of the contour as possible.
    2. If possible, the shape to be digitalized should be placed on a background with high
       contrast to the shape's colors. Black felt has proven well-suited in the tests up to now.
       Furthermore, any flat object (not a reference object!) should be placed in the middle of
       the shape in order guide the autofocus of the camera correctly.
    3. With the devices used thus far, shapes in the size of approx. 1 m² were examined. With
       good lighting and contrasts and well-positioned L objects, precisions in the range of
       approx. 1 mm per m were reached. This corresponds to expectations; for with a size of
       3,000 mm by 2,000 mm and a camera resolution of 12 Megapixels, there are approx.
       5,000 pixels in the length, that is, approximately 1.5 pixels per mm available. Thus
       theoretically, a deviation in the 1-2 mm range is possible.




3.7. Notes
This performance description is a snapshot in a stage where practical experiences exist using a
prototype. The everyday feasibility and maximum achievable precision now have to be examined
continuously in the course of deployment by additional customers.




A+W Software GmbH                      EN-FUNC-A+W iShape.docx                                     7
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH               EN-FUNC-A+W iShape.docx   8

