---
title: "A+W Business Delivery Reliability Guide"
source: "AWB_Delivery_Reliability_Guide.pdf"
tags: ["A+W Business", "Delivery Reliability", "User Guide", "Software", "Order Management", "Delivery Date", "Statistics", "Master Data"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A user guide for the A+W Business software, focusing on the Delivery Reliability functionality. It explains how to manage, track, and analyze delivery dates, differentiate between customer-requested and company-caused delays, and use the system's statistics for delivery date compliance."
long_description: "This user guide provides detailed instructions for working with the A+W Business Delivery Reliability feature. It is intended for users who manage orders and track delivery performance within the A+W Business software for the glass and windows industry. The document begins by explaining the backend data storage, detailing the difference between 'Planned shipping date' and 'Actual shipping date.' It guides users on how to display these dates in the order header for better visibility. The guide walks through the process of creating a document and then explains how to handle different scenarios for changing a delivery date, such as a customer requesting a later delivery versus a delay caused by the company (e.g., production issues). It provides step-by-step instructions on how to use the 'Document data' function to correctly record delays, ensuring that delivery reliability statistics accurately reflect the cause. The document also covers how to use the statistics module for delivery date compliance, including setting up filters, evaluation limits, and exporting data to CSV. Finally, it outlines the necessary master data settings, such as creating 'Reasons for postponement,' and configuring the system to prompt for a reason when a delivery date is changed after a certain order status is reached."
---

# User guide for working with A+W Business Delivery Reliability

---
## Contents
- The backend (behind the scenes)
- Displaying the dates on the order header
- Creating the document
- The different delivery date values
  - Customer requests later delivery
  - Delayed delivery caused by you
- Changing the delivery date
  - Customer requests a later delivery date
  - Delayed delivery caused by you
- Statistics for delivery date compliance
- Master data settings
  - Reasons for postponement
  - Entry in history if delivery date change after status X

## The backend (behind the scenes)

To understand how the delivery date works you need to have a basic understanding about how the delivery date data is stored. When you set a delivery date on an order header in the background there are two date values:

-   **Planned shipping (delivery) date**
-   **Actual shipping (delivery) date**

When the date is changed on an order header then both of these dates are changed to the same value. The planned delivery date is used to store the date that was originally set on the order which is used to calculate the date that the customer has requested.

Actual shipping date is the same as the planned shipping date until it is changed via the "Document data" function. For the two values to be different (to indicate a delayed delivery) you need to change the "actual shipping date" via this function since changing it on the order header will change both planned and actual to the same value which will have the effect that the system will not indicate that this delivery was delayed.

### Displaying the dates on the order header

If you want to be able to see these dates values as you get started with using this functionality you can left click the top left corner of the table at the bottom, go to properties and then you can add in the columns for "Delivery date planned" and "Delivery date real" (you can disable/hide these when you are doing testing and you have learned how this works if you want to).

