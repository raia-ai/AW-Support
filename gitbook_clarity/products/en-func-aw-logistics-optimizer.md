---
description: "EN FUNC A+W Logistics Optimizer"
---



# EN FUNC A+W Logistics Optimizer

     Functional Description


A+W Logistics Optimizer




                              english
1. Content
1.   Content                                                                3
2.   Notes on this Document                                                 4
     2.1. Trademarks                                                        4
     2.2. Copyrights                                                        4
     2.3. Disclaimer of liability                                           4
3.   Performance Description                                                5
     3.1. Data                                                              5
     3.2. Description                                                       5
     3.3. Requirements                                                      5
     3.4. List of functions                                                 6
          3.4.1. Master data and parameters                                 6
          3.4.2. Import                                                     8
          3.4.3. Planning                                                   9
          3.4.4. Optimization                                              10
          3.4.5. Release                                                   12
          3.4.6. Dispatch and delivery monitoring                          12
          3.4.7. Rack management                                           14
          3.4.8. Statistics, analyses and evaluations                      15
          3.4.9. Reporting to the A+W ERP system                           16
          3.4.10. Smart Delivery                                           16
     3.5. Limitations                                                      17
          3.5.1. Master data                                               17
          3.5.2. Import from the ERP system                                17
          3.5.3. Planning                                                  17
          3.5.4. Optimization                                              18
          3.5.5. Release                                                   18
          3.5.6. Delivery and delivery monitoring                          19
          3.5.7. Rack management                                           19
          3.5.8. Statistics and analyses                                   19
          3.5.9. Reporting to the ERP system                               20
          3.5.10. Smart Delivery / Delivery App                            20
4.   Contact Address                                                       21




A+W Software GmbH                   EN-FUNC-A+W Logistics Optimizer.docx        3
2. Notes on this Document
This documentation and the software described in it are only licensed and may only be used and
copied pursuant to this license. The contents of the documentation are for information purposes
only and are subject to changes without prior notice. The text and illustrations were compiled with
the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH assumes no
liability for errors or imprecise statements unless these can be traced back to intentional or
negligent actions.


2.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered
trademarks or other industrial property rights of third parties. The property rights of third parties
must be observed.


2.2. Copyrights
© 2019, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation can be copied, completely or in part, saved in an
archiving system, or transferred in any other form only in accordance with our license agreement.
Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by
recording or in any other way, without the written prior approval of A+W Software GmbH.


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




A+W Software GmbH                EN-FUNC-A+W Logistics Optimizer.docx                              4
3. Performance Description
3.1. Data
 Product              A+W Enterprise / A+W Business / A+W Business Pro
 Module               200100
 number
 Module               A+W Logistics Optimizer
 Description          Creates and/or optimizes the shortest routes and calculates
                      their costs
 Available            A+W Enterprisev6 / A+W Business v6 / A+W Business Pro v6


3.2. Description
The A+W Logistics Optimizer creates and optimizes the shortest routes – taking into consideration
your real fleet and the order data transmitted. The system will then tell you – taking into
consideration route limitations (e.g. bridge height or permissible vehicle weight) and traffic
information the optimal route with the optimal sequence of delivery points. Deviating delivery
addresses can also be considered, as are specific time and date promises made to your customers.
The total weight of the goods to be delivered is distributed across the trucks, in order that each
drop-off point only has to be visited once and in this way, the most suitable vehicle is always
selected for the route to be covered.
On the one hand, our solution offers you the opportunity to plan quickly and easily; on the other
hand, to find the optimal delivery result and fine-tune it using different options and parameters.
The planned costs are calculated for the routes (time, personnel, fuel, tolls), and these can be
compared to the actual costs after successful delivery. The system offers you its own
comprehensive statistics and analysis tool for this.
However, the A+W Logistics Optimizer supports not just route planning and evaluation, it also
assists you with delivery itself. Thus on the one hand you can export the route data to the
navigation system; on the other hand, you can use the program's own delivery app on a mobile
phone to book the delivery and report it back to the office in real time. There, the dispatch
manager can monitor the delivery of the route online and react directly to reports such as Sheet
0815 broken. The delivery and pick-up of racks can also be recorded with the A+W Logistics
Optimizer. The pick-up of racks can be planned into the routes.


3.3. Requirements
    •   A+W Enterprise (price list module 200002), A+W Business (price list module 210001) or
        A+W Business Pro (price list module 230001)
    •   Set-up and correct master data (for example, trucks, drivers)




A+W Software GmbH               EN-FUNC-A+W Logistics Optimizer.docx                                 5
   •   Required for a deeper integration in the sense of data transmission and feedback: the
       transfer of and reporting to the upstream commercial ERP system about the A+W
       Logistics Service must be configured correctly.
   •   ERP status points must be set up correctly for the reporting so that the order status is
       increased automatically based on the steps in the A+W Logistics Optimizer
   •   Parameters and switches in the route planning/generation and calculation must be set up
       and configured correctly (e.g. company location, time of standard route beginning, max.
       platform times).
   •   For a deep understanding and thus efficient application and optimal results, a 1-day
       training and intensive study of the manual are recommended.
   •   If possible, the customer should have its own shipping manager, who focuses deeply and
       regularly on the topic of dispatch logistics.
   •   The main problem to be solved should be in the area of dispatch logistics and no focus on
       the loading of trucks, for example with oversized sheets. For this, an integrated cargo
       space optimization is required, which the program does not include in the stage of
       expansion described here.
   •   If possible, there should be an in-house truck fleet – no delivery by carriers.


3.4. List of functions
3.4.1. Master data and parameters
   •   It is necessary to store individual master data in the system for: trucks, drivers, rack types,
       customers/target addresses
   •   It is possible to maintain your own master data for customers/target addresses in the
       system – thus it is possible at loading/unloading stations to map to which ones deliveries
       are made regularly although they are not stored in the ERP system as market partners (for
       example, construction sites)
       -   It is possible to store specific delivery times per customer in the master data; these
           are used in the course of route planning and optimization. Alternatively, you can
           enter/change delivery times per route, per delivery address manually.
       -   It is possible to define customers as priority customers in the master data. This way,
           they are assessed as especially important in the optimization. If a truck is overloaded,
           then the priority customers are given priority consideration. Alternatively, it is
           possible to define a customer as priority per route, per delivery address.
   •   It is possible to store individual master data for rack types in the system if you would like
       to use the possibilities for rack management – for unloading and loading of (empty) racks.
       -   If new rack types should be transferred to the A+W ERP system in the course of the
           order import, then the master data will be created accordingly automatically in the
           A+W Logistics Optimizer.
   •   It is possible to change the mode of optimization. This way, the system can either use pre-
       defined route information from the ERP system and just optimize the routes



A+W Software GmbH               EN-FUNC-A+W Logistics Optimizer.docx                                 6
       (Route_Origin) or, based on the order information itself, it can generate routes and then
       optimize them (DVA mode). This function mode is coupled to a license.
   •   In DVA mode, the minimum number of adjacent addresses are considered for the
       automatic generation of delivery areas and routes (for example 3 adjacent addresses to
       define a delivery area). The number of min. adjacent addresses can be defined. For this,
       the system uses a permanently defined and unchangeable calculation value for the
       distance calculation of each address point to each other address point in order to identify
       sensible neighbors and thus delivery areas.
   •   It is possible to set in the system whether primarily the order data/order addresses
       should be considered or the customer addresses/target addresses stored in the A+W
       Logistics Optimizer.
   •   It is possible to set whether the customer addresses are considered as delivery addresses
       or deviating delivery addresses in the order. In addition, it is possible to change delivery
       addresses manually in the planning step.
   •   It is possible to define the general route beginning (time and place) that should be
       considered for all routes in the master data. In the planning step, a deviating route
       beginning can be stored per route (time and place).
   •   It is possible to define the maximum platform time that should be considered for all
       routes in the master data. In the planning step, a deviating max. platform time can be
       stored per route.
   •   It is possible to define default values/settings for the route optimization in the parameters
       (e.g. fastest vs. shortest route). These settings can be overridden per route in the planning
       step.
   •   It is possible to switch the language while the program is running.
   •   It is possible to adjust the translations of the program yourself in order to use company-
       specific terms in the system, for example.
   •   Addresses that are transmitted via order import from the ERP system to the A+W Logistics
       Optimizer can be stored as "customers" in the Logistics Optimizer. Thus it is possible to
       load addresses quickly and easily, for example, for the pick-up of empty racks, without
       having to enter an order in the ERP system for this.
   •   It is possible to define the parameters for the route optimization:
       -    Time – optimization for fastest distance
       -    Distance – optimization for shortest distance (only for car)
       -    Date – optimization of the distance taking delivery times into consideration
       -    Priority - optimization of the distance taking prio customers into consideration
       -    A mix of these parameters is possible and makes sense. Here, the individual
            parameters can be weighted differently (in%). The total weighting of all parameters
            always corresponds to 100%.
   •   It is possible to store departments in the system. This function can be used, for example,
       to distinguish your own trucks from carriers' trucks and to limit costs.
   •   It is possible to store maintenance dates for trucks. If a truck is in maintenance, then it is not
       considered for the route planning on this day.


A+W Software GmbH                EN-FUNC-A+W Logistics Optimizer.docx                                   7
3.4.2. Import
   •   The import of data from the ERP system is possible in A+W Business /A+W Business Pro
       from the number manager. The import of data from A+W Enterprise is done from the
       shipping control.
   •   During the import, the address data is checked to ensure it is correct and the latitude and
       longitudes of the addresses are determined.
   •   In DVA mode, delivery areas are generated automatically during import, based on the
       number and position of the delivery addresses.
   •   If a customer should have placed several orders with the same delivery address, then
       these orders are grouped – and combined in the one delivery address. Thus a delivery is
       made to each address only once.
   •   For the route planning and assignment of trucks, only the address data and the weight to
       be delivered from the orders (incl. racks) are considered, as well as the delivery date per
       order.
   •   It is possible to import delivery addresses via csv files (please note that this way, no
       reporting of status information to the ERP system is possible!)
   •   The system generates the routes within the delivery areas using the delivery dates,
       addresses, and the glass weight of the orders to be delivered.
   •   During import, it is possible to select individual/specific trucks and to specify the delivery
       areas. Alternatively, the system's suggestions can be accepted/taken over.
   •   With active automatic delivery area generation, the system initially generates the delivery
       areas in hierarchical mode. The mode can then be changed in the course of planning.
   •   In the course of the import, the following data is transferred by A+W ERP system to the
       A+W Logistics Optimizer:
       -   Customer name
       -   Customer address
       -   Delivery address (if different from customer address)
       -   Delivery date
       -   AWB route number
       -   Glass weight in kg
       -   Order number
       -   No. of Orders
       -   Number of items per order and respective item number
       -   Number of sheets per item
       -   Glass weight per item
       -   Glass dimension per item (height and width of the sheets)
       -   Glass type per item (glass type designation)
       -   Rack numbers


A+W Software GmbH               EN-FUNC-A+W Logistics Optimizer.docx                                    8
       -   Rack types (these are then compared to the rack master data in the A+W Logistics
           Optimizer so that the rack parameters necessary for the cargo space optimization are
           pulled)
       -   Distribution order – item – shipping rack (in case of booking via A+W Barcode
           Manager)


3.4.3. Planning
   •   It is possible to shift (manually) orders/delivery addresses from one route/delivery area to
       another route/delivery area. This also applies for orders/delivery addresses that are on
       another delivery date (but have already been imported).
   •   It is possible to change the delivery date for orders and whole routes. (Note: this is not
       recommended. If the changing of delivery dates should be necessary, this should first be
       done in the A+W ERP system).
   •   It is possible to view details of the delivery addresses and the grouped orders in them.
       Some of these details can be changed/corrected (for example, the address data).
   •   It is possible to store additional weight and loading weight for a delivery address (for
       example, pick-up of empty racks).
   •   It is possible to plan and drive a route lasting several days. In this case, adherence to the
       break and driving times is the responsibility of the driver.
   •   In the planning step, it is possible to change the address data for a delivery point. The
       included, grouped orders within this delivery point cannot be changed individually in the
       process.
   •   It is possible to change and/or add individual parameters per delivery address – for
       example, max. unloading time on-site, additional contact information for the driver.
   •   It is possible to add more delivery addresses to a route and thus to reference customers
       from the customer base of the A+W Logistics Optimizer (that is, you can deliver
       something to a familiar customer address or pick something up there without having to
       enter an order). This is not reported back to the upstream ERP system.
   •   It is possible to specify a time per delivery address when the delivery should be made and
       a time window for how long the driver has to unload the goods.
   •   If in the included rack management there are racks to be delivered and/or picked up –
       with appropriate address – these racks can be added to the routes. Either the racks are
       added to the delivery addresses for the orders to be delivered or an additional stopping
       point is created within the route.
   •   It is possible to plan the same orders several times and optimize them with different
       parameters in order to get different alternative results. The route/alternatives can then
       be selected in the course of releasing the route that "best" fulfill the expectations.
       Planning alternatives (routes) that are not driven should be deleted (manually) in order to
       prevent conflicts (trucks assigned to different route alternatives at the same time).
   •   It is possible to return after optimizing the planning in order to change parameter and/or
       plan data (for example, additional directions for the driver and/or delivery times). If
       route/delivery-relevant data (times and/or address data) is changed, then there is a re-
       optimization in the next step.


A+W Software GmbH               EN-FUNC-A+W Logistics Optimizer.docx                                   9
   •   After the import, it is possible with active dynamic route generation, to change the mode
       of the generation. Thus it is possible to select from among 3 different algorithms/modes,
       which the system uses to generate the delivery areas (taking into account the total order
       weight incl. racks to be delivered and the existing trucks):
       -   Hierarchical mode
       -   EM Mode (Expectation maximization)
       -   Balanced Load This tries to load the truck evenly without splitting orders. Delivery is
           made only once to each address.
       -   Post code. In the process, routes are formed by postal code areas. This is especially
           recommended for delivery in large cities.
       -   The Hierarchical and EM mode distinguish themselves in the calculation algorithm
           with respect to the distance factor between delivery addresses in order to group
           several delivery addresses in one delivery area. With a change between the modes,
           the delivery areas are re-built differently.
       -   The Balanced Load mode distributes the order weight to be delivered evenly across
           the available trucks. Orders are thus not split, a grouping of orders with the same
           delivery address is not eliminated (each address is delivered to once). This mode
           distributes the delivery addresses to be driven to across the delivery area. Therefore,
           this mode only makes sense if you are delivering to customer in a relatively small
           delivery area.
       -   If empty racks should be available for pick-up, then the A+W Logistics Optimizer will
           report this in the course of order import. The user can then decide whether the pick-
           up address is added to the route automatically.


3.4.4. Optimization
   •   It is possible to consider statistical traffic information for the optimization – for example,
       long-term construction sites or traffic jam information. This data must be available to
       Nokia maps
   •   The system consider the maximum permissible driving period per driver.
   •   The system considers the country abbreviations stored in the master data for a country or
       border-spanning distance optimization and toll cost calculation.
   •   It is possible to pre-set the optimization parameters in the system's master data. In the
       course of the optimization, these can be changed per tour. The following options and
       parameters are available:
       -   Distance factor
       -   Weight factor
       -   Date factor
       -   Priority factor
       -   Time factor
   •   It is possible to change the route calculation mode (fastest vs. shortest) in the course of
       the optimization.


A+W Software GmbH               EN-FUNC-A+W Logistics Optimizer.docx                                 10
       -   The shortest mode is not supported for trucks, only for cars. Due to the truck
           restrictions, it is not possible to drive on all roads. Thus the shortest route is only
           available for cars. This is a restriction of Nokia Maps.
       -   After switching the mode, the alternative optimization results are listed. This way the
           user can select the best result for him.
   •   Using the optimization mode, it is possible to set how the system should plan and
       optimize a distance. Thus, for example, it is possible to completely avoid highways or to
       assign them penalty points. The following optimization modes are available in the course
       of the optimization per route:
       -   Route Mode
       -   Tunnel Mode
       -   Toll Mode
       -   Toll Mode
       -   Highway Mode
       -   Ferry Mode
       -   Train Mode
   •   The optimization considers the settings stored during the planning with respect to
       maximum delivery duration and delivery time. Please note that if necessary, the
       optimization parameters for this must be adjusted for the route, so that time is evaluated
       more highly as a criterion than, for example, the shortest or fastest route.
   •   It is possible to repeat the process steps for the planning and optimization for a route
       several times and to change parameters until the best result has been determined.
       -   As another possibility for multiple-alternative optimization, the Simulation mode was
           created. Here it is possible to do optimizations with different parameters and then to
           select the best (time, costs) from a list of all optimizations. Thus, an alternative
           optimization using the company's own trucks vs. Carrier and a Make-Or-Buy user
           decision based on this is possible.
   •   The system contains a cargo space optimization for trucks in order to consider and
       optimize the loading with racks and sheets. Necessary for this are rack bookings via A+W
       Barcode Manager (sheet on rack) or manual rack booking in the A+W ERP system.
       Considered during the cargo space optimization:
       -   Different rack types with respect to length and width
       -   Surrounding rectangle for overlarge sheets on rack
       -   Sequence of the unloading and loading stations according to route optimization
       -   Safe distance between individual racks
   •   The system calculates the planned driving and arrival time per address.
   •   It is possible after initial optimization to change the sequence of the delivery stations
       manually. The system then re-optimizes the route automatically.
   •   Based on the costs and consumption parameters stored in the master data (truck, driver),
       the system calculates the planned costs in the course of the optimization per route. After



A+W Software GmbH               EN-FUNC-A+W Logistics Optimizer.docx                                 11
        completion of a route driven, these can be compared to the actual costs and evaluated
        statistically.
    •   The following individual costs are calculated and summarized for a route:
        -   Toll Costs
        -   Driver costs (distance/time)
        -   Truck costs (gasoline consumption per 100 km, gasoline costs per liter)
        -   Fixed Costs
        -   Extra costs (other)
    •   The system can calculate various scenarios with regard to distance and costs. This is
        supported by the simulation mode, in which several alternatives can be calculated and
        optimized - among other things, using the company's own trucks or delivery by carriers.
        This offers the basis for a make-or-buy decision on the part of the user.


3.4.5. Release
    •   It is possible to export additional documents from the system for the driver (to upload
        them into the cloud). For this, a cloud address must exist and the document must be
        loaded to this cloud share (for example, DropBox). In A+W Logistics Optimizer, the link to
        this external address can be communicated to the driver (exported).
    •   If in the course of release conflicts should occur, for example, vehicle planned in parallel
        on different routes, then it is possible to resolve the conflict in the course of release
        through manual changes (for example, select another truck and/or driver manually)
        without having to re-optimize.
    •   It is possible to export optimized routes to a navigation system. Supported are TomTom
        and/or Garmin, as well as navigation function via here.com, which is integrated in the
        delivery app.
    •   It is possible to reset the status of routes that have already been released, to change
        them (for example, add or delete addresses) and re-release them. This also allows the
        changing of a route that has already been driven by a driver. After changing a route, it can
        be re-released. The delivery app then updates the data for the driver. Please note: only
        route sections and stations can be changed that have not yet been reached/booked.


3.4.6. Dispatch and delivery monitoring
A+W offers drivers its own delivery app. This app is available free of charge in the Google Play
Store for Android devices (e.g. Samsung). For iOS devices (e.g. Apple iPhone), an identical html
version (via html browser, e.g. Google Chrome or Safari) can be used.
    •   The A+W delivery app offers the following functional scope:
        -   Electronic signature
        -   Status of the dispatch (delivered, partially delivered, acceptance declined)
        -   Electronic text brief messaging (e.g. sheet #0815 broken)
        -   Selection of individual orders for partial delivery


A+W Software GmbH                 EN-FUNC-A+W Logistics Optimizer.docx                             12
       -   Display of route information and order information (e.g. weight, address)
       -   Display of the route on a map
       -   Display of the racks on the truck according to cargo space optimization
       -   Booking of racks for the integrated rack management (delivery and pick-up)
       -   Creation and linking of photos with respect to an order item (for example, for
           delivery of a rack to a construction site or photo of a broken sheet). The
           corresponding photo is reported back to the office via cloud and can be saved and
           evaluated together with the electronic signature.
       -   Navigation function from the current location to the next planned route address with
           here.com.
       -   Report of broken sheets (order, item, number) to the delivery monitoring in the
           office.
       -   Scanning of rack barcodes for delivery or pick-up of racks (note: for the delivery of a
           rack to a planned delivery address, no scanning is required. For this, only the
           unloading of the rack at the address must be confirmed with [OK]. This also applies
           for the planned pick-up of an empty rack at a planned address. The scanning of a rack
           barcode offers only an additional possibility for booking delivery and pick-up of racks
           - unplanned).
   •   In addition to the A+W delivery app, A+W offers the possibility to export data to an
       external truck GPS system and to receive and evaluate the route information in real time
       from these systems. Thus, for example, it is possible to receive the following data, read it
       out automatically and evaluate it:
       -   The current actual location of the truck
       -   Consumption data
       -   Speed
       -   Violations, e.g. of the platform times and breaks
       The connection to the third-party system from SkyeEye (http://skyeyegps.com) and/or
       Atlantis (http://www.atlantis-technology.com) is supported. Furthermore, it is possible to
       connect the system providers GEOMBO and TomTom Webfleet.
   •   Thanks to the incorporation of a truck GPS system and the associated coupling to the
       truck's on-board computer, the actual costs of a route can be determined and compared
       automatically to the planned costs. This assists with route analysis and statistics.
   •   If there is no truck GPS system available or there is no connection to the truck's on-board
       computer, the actual costs can be entered manually after completion of the route. For
       this, the actual delivery duration and distance can be entered into the route costs using
       the driver's report.
   •   During the delivery of the route, the driver can be monitored in the office. Here, it is
       possible to view the following information in real time:
       -   Display of the route on a map
       -   Display of the position and time stamp of the location from which and when the
           respective booking was made by the driver
       -   Display of text messages by the driver (e.g. sheet #0815 broken please remake)


A+W Software GmbH               EN-FUNC-A+W Logistics Optimizer.docx                              13
       -   Display of the customer's electronic signature
       -   Colored marking of the delivery addresses for display of a delivery made (green) or
           deliver declined/partially declined (yellow)
       -   If GPS is active in the truck (smartphone, truck GPS system), the truck's current
           position on the route is visible
   •   The route can be supported with a navigation device (TomTom or Garmin).
   •   Alternatively (more cost-effectively), the A+W delivery app is coupled to the navigation
       app from here.com (BMW). Thus it is possible to map the announcement and display of
       the route (for example, turn left in 100 m) purely on a mobile phone.
   •   It is possible to change delivery addresses after the data for delivery has been released
       (e.g. to the driver app) – e.g. if there have been last-minute changes to the delivery
       address. For this, the route must be loaded again in the office, it can then be changed and
       uploaded again to the cloud. The delivery app then connects automatically to this new
       data (note: only possible for delivery addresses that have not been driven to yet).
   •   It is possible to add additional stop addresses or to delete stop addresses. For this, the
       route must be loaded again in the office, it can then be changed and uploaded again to
       the cloud. The delivery app then connects automatically to this new data (note: only
       possible for delivery addresses that have not been driven to yet).
   •   It is possible to change delivery addresses after the data for delivery has been released
       (e.g. to the driver app) – e.g. if there have been last-minute changes to the delivery
       address. For this, the route must be loaded again in the office, it can then be changed and
       uploaded again to the cloud. The delivery app then connects automatically to this new
       data (note: only possible for delivery addresses that have not been driven to yet).
   •   It is possible during the route to update data and/or the route, e.g. if the driver reports
       that he's stopped in a traffic jam and all other delivery addresses to be driven to are
       delayed by time x. For this, the route must be loaded again in the office, it can then be
       changed and uploaded again to the cloud. The delivery app then connects automatically
       to this new data (note: only possible for delivery addresses that have not been driven to
       yet).
   •   It is not possible to take a photo of the delivery within the delivery app (e.g. frame at
       unloading station or photos of broken sheets) and report back to the office. Information
       of this type must be created and transferred independent or and outside the delivery app.
   •   Thanks to the online connection and monitoring of delivery via the delivery app, the
       booking time stamp of a delivery/pick-up is transmitted to the office and it can therefore
       be compared to the planned data. This is done automatically for the route analysis
       (individual route) and statistics (route-spanning).


3.4.7. Rack management
   •   A small, stand-alone rack management is integrated into the current version of the A+W
       Logistics Optimizer. This is coupled to the rack management of the A+W ERP system and
       enables the following functions:
       -   Transfer of the rack information together with the order information (conditions a
           sheet/item rack assignment with A+W Barcode Manager)



A+W Software GmbH               EN-FUNC-A+W Logistics Optimizer.docx                                14
       -   For delivery of a rack via delivery app, there is an outgoing rack booking in the A+W
           ERP system.
       -   For pick-up of a rack via delivery app, there is an incoming rack booking in the A+W
           ERP system.
   •   It is possible to create racks for delivery and/or pick-up. For this, the address and date, as
       well as the parameters of the rack can be stored (for example, dimensions and weight).
   •   Created racks – or rather the addresses for these racks – can be added to a route. For this,
       the system automatically displays a notice as soon as route is planned for a day and racks
       for delivery or pick-up have also been created for this day.
   •   Using the delivery app, the deliver and/or pick-up of the racks can be booked on the go.
   •   In the course of program expansion and diversification of A+W Smart Delivery, the
       data/data structures transferred by A+W ERP system to the A+W Logistics Optimizer have
       been expanded. Thus, information about the rack loading (order - order item - rack(s)) is
       also transferred. For this, it is necessary to book the sheets of an item to one or several
       racks via A+W Barcode Manager. In the course of this data transfer, the necessary rack
       information is transferred the appropriate rack is created in the A+W Logistics Optimizer.
       This rack can then be delivered in the course of a route and later picked up on another
       route. Therefore, it is known which sheets of an order item are on which and how many
       racks.


3.4.8. Statistics, analyses and evaluations
   •   In the current version of the A+W Logistics Optimizer, the system includes its own analysis
       tool for evaluating an individual route driven. This analysis tool offers the following
       possibilities:
       -   Evaluation of an individual route with respect to the deviations between planned and
           actual values (e.g. driver costs, consumption, time and distance deviations)
   •   In addition, an individual, separate statistics module is integrated. It has no
       connection/coupling to the ERP and/or PPS statistics (e.g. A+W Business Statistics). The
       statistics module offers the following possibilities for adding up and evaluating.
       -   It is possible to filter on individual parameters – route status, driver level, truck level,
           customer level. Here there are numerous filter possibilities. Data is also displayed
           both numerically and graphically.
       -   It is also possible to compare different departments to one another. This can be used,
           for example, to compare delivery with the company's own truck to delivery by
           external carriers.
       -   It is possible to export individual statistical data and evaluations to MS Excel. This
           way, you can import this data into the ERP system, data warehouse or BI tool and
           continue processing it.
       -   Please see the individual possibilities for the statistics and analysis in the A+W
           Logistics Optimizer manual.
   •   The system supports the output of reports. This is done with the incorporation of SAP
       Crystal Reports®. Thus it is also possible to output customer-specific reports.



A+W Software GmbH               EN-FUNC-A+W Logistics Optimizer.docx                                 15
   •   No pre-defined A+W standard reports are included in the package price for the A+W
       Logistics Optimizer.
       -    Loading list
       -    Delivery list (display of all delivery stations and of the delivery status such as
            accepted, partially accepted, broken incl. order, item, and quantity of the broken
            sheets, electronic signature)
       -    Route list (display of all sections and orders/racks to be delivered per address)


3.4.9. Reporting to the A+W ERP system
   •   In the current version of the A+W Logistics Optimizer, the system writes the following
       information back to the A+W ERP system:
       -    Status of the delivery per order up to maximum delivery accepted or delivery refused
       -    Route ID
       -    Sequence (within the route)
       -    Name and customer address for rack delivery (note: there is an automatic outward
            rack booking)
       -    Name and customer address for rack pick-up (note: there is an automatic inward rack
            booking)


3.4.10.        Smart Delivery
In the course of program expansion and diversification of A+W Smart Delivery, the data/data
structures transferred by A+W Business to the A+W Logistics Optimizer have been expanded. In
addition, the product was designed to be scalable with respect to size and functionality:
   •   A+W Smart Delivery (name of the lowest stage of expansion corresponds to the data
       structure extension). In this stage of expansion, no map material and optimization are
       included; that is, it only includes the delivery app and an empty A+W Logistics Optimizer.
       The individual delivery addresses are transferred by A+W Business to the A+W Logistics
       Optimizer and they can be combined here into a route. The route information is
       transferred to the delivery app (via cloud). This way, the driver can use the delivery app to
       book the delivery of a route - incl. photos and electronic signature. The delivery can be
       traced and monitored in the office.
   •   A+W Smart Delivery Maps. In this stage of expansion, the map material is also included
       with the delivery app. This way, the delivery addresses can be combined into a route and
       displayed graphically on a map. This map information is also forwarded to the driver (via
       delivery app). An optimization of the sequence and route is not possible. For all booking
       functions of the delivery app, the geo-coordinates of the booking are determined and
       reported back to the office. Thus, for example, the precise location of a rack delivery can
       be booked and saved.
   •   A+W Logistics Optimizer. This stage of expansion includes all functions and data - incl.
       delivery app, map material, and optimization.




A+W Software GmbH               EN-FUNC-A+W Logistics Optimizer.docx                              16
3.5. Limitations
3.5.1. Master data
   •   It is not possible to transfer truck and/or driver-related master data from the ERP system
       to the A+W Logistics Optimizer. This data must be set up again.
   •   It is not possible to define additional, own master data that should be transferred via the
       A+W Logistics Service to the A+W Logistics Optimizer.
   •   It is not possible to store master data for several different locations in the system. The use
       of the A+W Logistics Optimizer is done on a single-site basis


3.5.2. Import from the ERP system
   •   It is not possible to transfer additional document attachments from the ERP system via
       order import to the A+W Logistics Optimizer – in order to view these in the A+W Logistics
       Optimizer and delivery app.
   •   It is not possible to transfer truck and/or driver-related information from the ERP system
       to the A+W Logistics Optimizer.
   •   Part-related information is not transferred. Only information on the order level and the
       item level is transferred.
   •   It is not possible to transfer orders whose status is higher than route optimized (since, for
       example, the optimization results were saved in the A+W Logistics Optimizer or the routes
       were released)back to the A+W Logistics Service. A reduction of the order status is not
       sufficient for this.
   •   It is not possible to split orders/items in the A+W Logistics Optimizer. The same type of
       delivery addresses must always be combined with the same delivery date. Splitting (for
       example, in case of partial deliveries) must always be done via the ERP system.
   •   It is currently not possible to transfer information about individual sheets (sheet barcode).
       After scanning 10 sheet barcodes for item 2 from order 0815 on rack 16, it is thus only
       known in A+W Smart Delivery/A+W Logistics Optimizer that 10 sheets from item 2 from
       order 0815 are on a rack 16.


3.5.3. Planning
   •   It is not possible to store break times in/for routes This is the driver's responsibility.
   •   It is possible to specify a time per delivery address when the delivery should be made and
       a time window for how long the driver has to unload the goods. Here it is not possible to
       store exact calculation (order quantity/weight corresponds to duration X) so that the
       system automatically calculates an unloading duration per target address and considers
       this for the planning.
   •   It is not possible to store in the system that the use of a crane and/or forklift is required
       for loading and unloading orders and/or racks. This is also not considered in the
       calculation of the loading and unloading times.



A+W Software GmbH                EN-FUNC-A+W Logistics Optimizer.docx                                  17
   •   It is not possible to divide up grouped orders (same customers, same delivery address,
       same delivery date) and to plan these on different trucks or deliver them to different
       addresses.
   •   In the planning step, it is possible to change the address data for a delivery point. The
       included, grouped orders within this delivery point cannot be changed individually in the
       process. This is conditioned by the grouping of the orders with identical delivery address
       and customer during import.
   •   Changes to the delivery address in the course of planning are not reported back to the
       ERP system.
   •   It is possible to add more delivery addresses to a route and thus to reference customers
       from the customer base of the A+W Logistics Optimizer (that is, you can deliver
       something to a familiar customer address or pick something up there without having to
       enter an order). This is not reported back to the upstream ERP system.
   •   In the course of the planning, different modes can be selected with which the system
       calculates the distances between the various delivery addresses. In order to identify and
       group neighbors this way, each mode (hierarchical, EM) has stored a fixed distance value.
       It is not possible to change this distance value.
   •   It is not possible to do location-spanning, multi-site logistics planning and optimization.
       A+W Software GmbH currently does not have a coherent concept for location-spanning
       logistics planning and delivery that would address the multitude of logistical and capacity
       requirements of a multi-site solution. However, a via-plant logic is supported through the
       possibility of inserting another branch office for loading and unloading on a route as
       intermediate address.


3.5.4. Optimization
   •   In the course of the optimization, it is not possible to make reference to real-time traffic
       information.
   •   During delivery/driving of the route, there can be no automatic follow-up/re-optimization
       after changes and/or messages from the driver. The system does not automatically re-
       plan (ex: the driver is stopped in a traffic jam and will be 2 hours late to the next delivery
       address). For a re-planning/recalculation of the route, its status must be reset in the
       office, changed, and then re-released.
   •   The system can calculate different scenarios with respect to distance and costs, however
       there is no automatic make-or-buy decision. The user must make this decision himself
       based on the costs determined. The user is assisted with this especially in simulation
       mode for planning and optimization.


3.5.5. Release
   •   It is not possible to transfer/export additional documents (e.g. delivery notes,
       accompanying documents) from the A+W Logistics Optimizer and/or the ERP system to the
       navigation system and/or the delivery app. However, it is possible to provide a link to an
       Internet address – so that documents can be uploaded to the cloud manually and this
       address can be exported and sent along.



A+W Software GmbH               EN-FUNC-A+W Logistics Optimizer.docx                              18
3.5.6. Delivery and delivery monitoring
   •   It is not possible for the driver to independently re-plan the route, for example because
       he's sitting in traffic or a delivery address is added or omitted. This has to be done by the
       office. Here, a route can be re-planned and re-released. The driver's delivery app
       automatically loads the new data.
   •   There is no automatic re-planning of a route if the driver is sitting in traffic, for example.
       This has to be done by the office. Here, a route can be re-planned and re-released. Here,
       taking into consideration delivery times and priorities, a decision is made whether
       delivery addresses should be omitted or how the sequence of the delivery addresses
       should be changed. The system helps in the course of planning and optimization. As soon
       as a route has been changed accordingly, it can be released again. The driver's delivery
       app then automatically loads the new data.


3.5.7. Rack management
   •   It is not possible to transfer rack-related data from the A+W Rack Manager (location-
       spanning rack management incl. invoicing and dunning).
   •   It is not possible to transfer data with respect to the delivery or pick-up of racks from the
       A+W Logistics Optimizer to the A+W Rack Manager.
   •   It is not possible to scan the barcodes of individual sheets so that they can be processed in
       the A+W Logistics Optimizer. The processing of data currently takes place on the item
       level. This way, for example, breakage can be booked - order 08 - item 15 - 2 of 10 sheets.
   •   The system does not currently consider any data from the A+W Rack Optimizer (alias
       PMO). Therefore, it is not known where on a rack an individual sheet is located. It is
       currently only known that a quantity of x sheets of an order item is on a rack.
   •   It is currently not possible to store parameters for the precise characteristics of a rack
       (e.g. number of slats, distances, etc.).
   •   It is currently not possible to store whether a fork lift or crane is required for loading or
       unloading a rack.
   •   A coupling with the Gestellpool Europe does not currently exist and is not possible.


3.5.8. Statistics and analyses
   •   It is not possible to export statistical data and/or evaluations directly (e.g. via Web
       service) to the ERP system, a data warehouse or a BI tool. Here, the path via an Excel
       export and import is possible.
   •   It is not possible to set up individual/new filter and selection options for statistics
   •   Please see the individual possibilities for the statistics and analysis in the A+W Logistics
       Optimizer manual.




A+W Software GmbH               EN-FUNC-A+W Logistics Optimizer.docx                                   19
3.5.9. Reporting to the ERP system
   •   Order status that is higher than route optimized (delivery accepted, acceptance refused,
       route completed, route archived, route deleted) is not currently reported back to the
       A+W ERP system A+W Enterprise.
   •   Delivery status that is higher than delivery accepted/acceptance refused (route
       completed, route archived, route deleted) is not currently reported back to the A+W ERP
       system A+W Business.
   •   The electronic signature is not reported back to the ERP system.
   •   Pictures/photos of the delivery app are not reported back to the ERP system.
   •   Route costs are not reported back to the ERP system (neither planned costs nor actual
       costs).
   •   Breakage information is not reported back to the ERP system.
   •   It is not possible to report additional, freely-definable information back from the A+W
       Logistics Optimizer to the upstream ERP system.


3.5.10.        Smart Delivery / Delivery App
   •   There is currently no IOS version of the delivery app available. Alternatively, the html
       version can be used via installed browser. This html variant offers the same functional
       scope as the Android version of the delivery app.
   •   A coupling of the delivery app with the Gestellpool Europe does not currently exist and is
       not possible.




A+W Software GmbH              EN-FUNC-A+W Logistics Optimizer.docx                               20
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH               EN-FUNC-A+W Logistics Optimizer.docx   21

