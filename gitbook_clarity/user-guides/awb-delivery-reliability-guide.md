---
description: "AWB Delivery Reliability Guide"
---



# AWB Delivery Reliability Guide

User guide for working with A+W Business Delivery Reliability

Contents
 The backend (behind the scenes) ............................................................................................................. 1

    Displaying the dates on the order header .............................................................................................. 1

 Creating the document .............................................................................................................................. 2

 The different delivery date values ............................................................................................................. 2

    Customer requests later delivery ........................................................................................................... 2

    Delayed delivery caused by you ............................................................................................................ 2

 Changing the delivery date ........................................................................................................................ 3

    Customer requests a later delivery date ................................................................................................ 3

    Delayed delivery caused by you ............................................................................................................ 5

 Statistics for delivery date compliance ...................................................................................................... 9

 Master data settings ................................................................................................................................ 13

    Reasons for postponement .................................................................................................................. 13

    Entry in history if delivery date change after status X.......................................................................... 14
The backend (behind the scenes)
To understand how the delivery date works you need have a basic understanding about how the delivery
date data is stored. When you set a delivery date on an order header in the background there are two
date values:

       Planned shipping (delivery) date
       Actual shipping (delivery) date

When the date is changed on an order header then both of these dates are changed to the same value.
The planned delivery date is used to store the date that was originally set on the order which is used to
calculate the date that the customer has requested.

Actual shipping date is the same as the planned shipping date until it is changed via the “Document data”
function. For the two values to be different (to indicate a delayed delivery) you need to change the “actual
shipping date” via this function since changing it on the order header will change both planned and actual
to the same value which will have the effect that the system will not indicate that this delivery was
delayed.

Displaying the dates on the order header
If you want to be able to see these dates values as you get started with using this functionality you can
left click the top left corner of the table at the bottom, go to properties and then you can add in the
columns for “Delivery date planned” and “Delivery date real” (you can disable/hide these when you are
doing testing and you have learned how this works if you want to).




                                                                                                 1|Page
Creating the document
First you create your order in AWB as you would normally do. In this example I have set the delivery date
to 22.03.2019:




Add your positions to the documents and follow your normal work procedure to get the confirmed order
sent to production.

The different delivery date values
When changing the delivery date values you need to keep in mind what your internal work process is and
if the delivery date is pushed back due to the customer calling and requesting a later delivery date or if it
is you as the producer/supplier that is the reason for the delay.

Customer requests later delivery
If the customer calls and requests a later delivery date which you choose to accommodate then you
would normally not consider this a delayed delivery that should affect your delivery reliability statics
negatively as a supplier in a negative way if the customer wants statistics on your delivery reliability.

Delayed delivery caused by you
If there is a delivery delay where you have had issues in your production or delayed shipment from your
supplier then it’s a real delivery delay and if you cannot ship to the customer on time then the statistics
should affect this. To show that there is a delivery delay that is your “fault” you will need to change the
delivery date via the “Document data” function.



                                                                                                   2|Page
Changing the delivery date

Customer requests a later delivery date
When the customer requests a later delivery date you can go to the order header and select the new
delivery date that you want to set. This will change both the planned and the real delivery date so that
there is no indication that you have caused a delivery delay at this point.

Original delivery date is 22.03.2019




                                                                                                 3|Page
The request from the customer is to change this to 27.03.2019. The status of the document is 400 and we
do have the setting active to request reason / comment for changes to delivery date if status of the
document is >= 400 (setting shown below):




Both the real and planned delivery date is now changed and the remark has been added to the comments
and is also available in the history of the document. The comment on tab 8 on the order header shows
the , the time it was done, by who, the reason, the comment and the date FROM -> TO.




This delivery date is now changed but will not affect your delivery statistics in a negative way since
planned and real is the same date.




                                                                                                  4|Page
Delayed delivery caused by you
Using the same order as an example we now have a scenario where we have a breakage in the factory,
and we won’t be able to produce the broken unit in time for delivery, so we need to push the delivery date
a few days. This is a delivery delay caused by a problem in the factory so we are responsible for the
delay and this should be indicated in the delivery reliability statistics.

Document data – Delaying the delivery the correct way
There are three ways to open document data
    From functions on document header
    From menu under the Documents section
    Right click on document in a number manger

When you have document data open then you can choose to change document by document by entering
the document number and applying the change or by loading a NM where you have all the orders that
needs to have their delivery delayed.

Per document
To change only one document I enter the order number in the “Number” (Marked in yellow) field and
press TAB or Enter so that the order’s data is loaded onto the screen.




                                                                                               5|Page
Then you select the new delivery date for the order and make necessary changes regarding status or
route. You can also select if you want the changed document to be added to a number manager so that
you keep track of the document you have changed.




You will be asked to enter a reason and a comment:




                                                                                          6|Page
The real delivery date is now updated and the planned date is kept:




Now you can also see how the values are stored on the order header, the delivery date and shipping date
looks the same, but the original shipping date values are stored in the background:




                                                                                            7|Page
You will also get the remark in the comment section under tab 8, customer info.




Per Number Manager
Open the “Document data” function where you have the document that you want to change/delay the
delivery date:




You should only have the document that you need to change the delivery date for in the NM.



                                                                                             8|Page
Keep in mind that the dates you select select when in “Number manager mode” will be applied to all
documents in the NM but but you can change the cause and comment per document.

Statistics for delivery date compliance
In the statistics for the delivery date compliance you can choose to check customers or suppliers. You
can also select if you want to check the archive databases as well as the main database or only a specific
archive year.




In the restrictions you can set a date interval and you can also specify a range of customer numbers (or a
specific customer number) as well as a customer group. You can also select all customer by using the
“Do not limit” option.




                                                                                               9|Page
The evaluation limits can be set however you need it to be. It is used in the summary of the data in the
table below that shoes the results:




The results can be printed via the menu at the top:




If you want to take this data and work with it in Excel for example then you can choose to export the data
to CSV by left clicking the upper left of the table and choosing the option to Write CSV file.




                                                                                               10 | P a g e
Explanation from the help file which can be opened via the F1 key from within the Delivery date
compliance statistics.




                                                                                             11 | P a g e
12 | P a g e
Master data settings
These settings are do need to be setup to be available for use. The reasons can be easily setup by you
as a customer but when it comes to changes in the company master data it is recommended that you
contact the A+W team to change this setting.

Reasons for postponement
These reasons can be setup to be selected as reason when there is a change to the delivery date. Press
“New”, enter Name of reason and then save to add reasons available for selection. Some example
reasons might be:

       Customer requested later delivery
       Production problems
       Breakages
       Delayed shipment from supplier




                                                                                            13 | P a g e
Entry in history if delivery date change after status X
It is possible to setup that the system prompts you to enter a reason and a comment if the delivery date is
changed after a certain status as been reached. The dialog shown prompts the user to enter a cause
(from the “Reasons for postponement of delivery date” mentioned above) and to enter a comment.

Be aware! This dialog looks the same as the one shown when changing the delivery date from the
“Document data” function but it will still change both the delivery date planned and delivery date real so
the system will not register this as a delivery delay (AWB version 13.4.523).




                                                                                               14 | P a g e

