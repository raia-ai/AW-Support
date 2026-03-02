---
description: "EN AWBusiness Statistics 4.01"
---



# EN AWBusiness Statistics 4.01

Statistics             F




                       english




             A+W Business
                                                                                                                Introduction




                                           Introduction
                                           This section of the documentation contains editorial notes.


                                           Revision overview
                                           Section           Description
                                           Version / Date

                                           1.00/03-1998      Original version

                                           2.00/08-2000      Reworking of statistics

                                           3.00/12-2003      Structural conversion to program structure 4.0

                                           3.01/08-2008      Correction of typos

                                           3.02/09-2008      Figure and section numbers adjusted.

                                           3.03/09-2010      Layout adapted to documentation concept 2010.

                                           3.04/01-2013      Layout adjusted to A+W Business.

                                           4.00/06-2016      Complete reworking

                                           4.01/01.2017      Product and company names adjusted.



                                           Editorial
                                           The editorial provides information on the following topics:
                                           •   Notes on this document
                                           •   Copyrights
                                           •   Trademarks
                                           •   Contacts

                                           Notes on this document
                                           This publication is written exclusively for end users of A+W Business.
                                           The documentation and software described therein are licensed only and must
                                           be used or copied only in accordance with the terms of our license agreement.
                                           The contents of the documentation are for information purposes only and are
                                           subject to changes without prior notice. The text and illustrations were com-
                                           piled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W
                                           Software GmbH assumes no liability for errors or omissions unless these are
                                           based on intentional or grossly negligent behavior.
                                           This document describes the full scope of A+W Business.
4.01 / 01-2017




                 A+W Business Statistics                                                                                 F-3
                 Introduction




                                Copyrights
                                © 2017, A+W Software GmbH, all rights reserved, including the right of reprint,
                                the production of copies and of the translation.
                                The documentation may be copied, completely or in part, saved in an archiving
                                system, or transferred in any other form only in accordance with our license
                                agreement. Transmission of the documentation is not allowed, neither elec-
                                tronically, nor mechanically, nor by recording or in any other way, without prior
                                written approval from A+W Software GmbH.

                                Trademarks
                                All hardware and software names mentioned in this documentation might also
                                be registered trademarks or other property rights of third parties. Copyrights of
                                third parties must be complied with.

                                Contacts
                                A+W Software GmbH

                                Am Pfahlgraben 4-10

                                D-35415 Pohlheim

                                   +49 6404 205 10

                                   +49 6404 205 1877

                                Zentrale@a-w.com

                                http://www.a-w.com
4.01 / 01-2017




                 F-4                                                                   A+W Business Statistics
                                                                                                                                                           Contents




                                           Contents
                                           Introduction ............................................................................................................. F-3
                                             Revision overview ............................................................................................... F-3
                                             Editorial ............................................................................................................... F-3

                                           Software Reference                                                                                                    F-7
                                           Overview ................................................................................................................. F-9
                                           Sales Statistics ..................................................................................................... F-10
                                             Order Information .............................................................................................. F-10
                                                Print menu ...................................................................................................... F-11
                                                Order Info – Options ...................................................................................... F-11
                                                Order Info – Entered ...................................................................................... F-15
                                                Order Info – Produced ................................................................................... F-16
                                                Order Info – Invoiced ..................................................................................... F-17
                                                Order Info – Open .......................................................................................... F-18
                                                Order Info – Graph ......................................................................................... F-19
                                             Selection ............................................................................................................ F-20
                                             Turnover Sales .................................................................................................. F-21
                                                Options menu ................................................................................................. F-21
                                                Super statistics menu ..................................................................................... F-22
                                                Turnover Sales – Selection ............................................................................ F-23
                                                Turnover Sales – Restrictions ........................................................................ F-28
                                                Turnover Sales – Table .................................................................................. F-29
                                                Turnover Sales – Graph ................................................................................. F-30
                                                Turnover Sales – SQL ................................................................................... F-31
                                             Super Statistics ................................................................................................. F-32
                                             Super Statistics – Export ................................................................................... F-34
                                             Super statistics – Import .................................................................................... F-35
                                             Complaints Statistics Sales ............................................................................... F-36
                                             Statistics by Structure ........................................................................................ F-37
                                                Statistics by Structure – Selection ................................................................. F-37
                                                Statistics by Structure – Table ....................................................................... F-40
                                             Customers by Order Area ................................................................................. F-42
                                           Purchasing Statistics ............................................................................................ F-44
                                             Turnover Purchase Statistics ............................................................................ F-44
                                             Complaint Purchase Statistics ........................................................................... F-45
                                             Delivery Date Compliance ................................................................................. F-46
                                             Consumption Analysis ....................................................................................... F-48
                                                Consumption Analysis – Selection ................................................................. F-48
                                                Consumption Analysis – Restrictions ............................................................. F-51
                                                Consumption Analysis – Table ...................................................................... F-53
                                           Commission Statistics ........................................................................................... F-54
                                           Intrastat Message ................................................................................................. F-56

                                           Part index                                                                                                         F-59
                                           Index ..................................................................................................................... F-61
4.01 / 01-2017




                 A+W Business Statistics                                                                                                                            F-5
                 Contents
4.01 / 01-2017




                 F-6        A+W Business Statistics
Statistics                  F

             Software Reference




              A+W Business
                 Software Reference                                                                              Overview




                                           Overview
                                           A+W Business offers various evaluation possibilities. Here, as described be-
                                           low, a distinction is made between current order stock evaluation, sales, com-
                                           plaint, and commission statistics.
                                           •   “Sales Statistics” on page F-10
                                           •   “Purchasing Statistics” on page F-44
                                           •   “Commission Statistics” on page F-54
                                           •   “Intrastat Message” on page F-56

                                               System settings
                                               In the company data, you can specify details for the transfer of the orders
                                               and purchase orders into the statistics. For a detailed description, see the
                                               Master data section.

                                                Master Data, “Company Data – Archives” on page B-931
4.01 / 01-2017




                 A+W Business Statistics                                                                               F-9
                 Sales Statistics                                                            Software Reference




                                    Sales Statistics
                                    The statistics in A+W Business provide an important instrument for company
                                    analysis. They include evaluations of your customers, industries, products,
                                    business areas, representatives, etc. For these evaluations, you can select
                                    whether you want to evaluate the data year by year or month by month.
                                    This chapter provides information on the following subjects:
                                    •   “Order Information” on page F-10
                                    •   “Selection” on page F-20
                                    •   “Turnover Sales” on page F-21
                                    •   “Super Statistics” on page F-32
                                    •   “Super Statistics – Export” on page F-34
                                    •   “Super statistics – Import” on page F-35
                                    •   “Complaints Statistics Sales” on page F-36
                                    •   “Statistics by Structure” on page F-37
                                    •   “Customers by Order Area” on page F-42


                                    Order Information
                                    Statistics > Order info
                                    On this dialog, you evaluate your order stock. Here you can distinguish be-
                                    tween the new orders, orders transferred to production, and invoiced orders.
                                    This dialog offers the following tabs:
                                    •   “Order Info – Options” on page F-11
                                    •   “Order Info – Entered” on page F-15
                                    •   “Order Info – Produced” on page F-16
                                    •   “Order Info – Invoiced” on page F-17
                                    •   “Order Info – Open” on page F-18
                                    •   “Order Info – Graph” on page F-19
4.01 / 01-2017




                 F-10                                                                   A+W Business Statistics
                 Software Reference                                                                        Sales Statistics




                                           Print menu
                                           Statistics > Order info
                                           Use this menu to start the printing of the evaluation on the screen or printer:
                                           •   Default:
                                               Opens the Selection dialog to specify which data should be printed.
                                                “Selection” on page F-20
                                           •   Sales:
                                               Starts the printing of the sales data and the comparison data from the pre-
                                               vious year. The work days are specified by month in the table display. The
                                               display closes with the values for the average sales per working day.


                                           Order Info – Options
                                           Statistics > Order info > Options tab




                                           Fig. F-1     Order info – Options


                                           On this tab, you specify the options for selection and output. The result of the
                                           search is output on the Entered, Produced, Invoiced, and Open tabs.
4.01 / 01-2017




                 A+W Business Statistics                                                                              F-11
                 Sales Statistics                                                                 Software Reference




                                    Columns
                                    Use the check boxes to specify the columns that should be displayed on the
                                    tabs.
                                    •   Qty:
                                        Total quantity of all order items in the selected period.
                                    •   Area:
                                        Total area of all order items.
                                    •   Lin. m.:
                                        Total length of all edges.
                                    •   SP:
                                        Total SP.
                                    •   PP:
                                        Total PP.
                                    •   Contribution margin:
                                        Total of the contribution margin. In the Selection criteria area, the options
                                        for the contribution margin are enabled.
                                     The column is not displayed.
                                     The column is displayed.

                                    Selection criteria
                                    In this area, you specify the selection criteria.
                                    •   Day, Month, Year, Calendar week, Quarter:
                                        With the selection of an option, you specify the period to be considered:
                                        The options Year and Quarter are locked if you have checked the Orders
                                        check box in the Break down by area.
                                        If you select the listing by period, the selection will be limited accordingly.
                                    •   Select date:
                                        With this setting, you limit the period to a particular set of dates.

                                    Classifier Only the classifiers are available that apply for all partners and/or
                                    customers.
                                     Master Data, “Classifiers” on page B-735

                                    Value from, Value to Limitation of classifier values.
                                     Master Data, “Classifier Value Allocation” on page B-780

                                    Contribution margin With the selection of the option, you specify whether
                                    the contribution margin should be displayed as amount or percentage. The
                                    fields are only enabled if the Contribution margin check box is checked in the
                                    Columns area.
                                     Master Data, “Classifiers” on page B-735
4.01 / 01-2017




                 F-12                                                                       A+W Business Statistics
                 Software Reference                                                                           Sales Statistics




                                           Value from, Value to Limitation to a value or a span of values. You can also
                                           enter negative values.

                                               Examples

                                               Entry                Result

                                               Negative value:      All orders whose costs are greater than the SP, e.g.
                                                                    from -99999 to 0.00

                                               Zero                 All orders whose costs are covered by the SP, e.g.
                                                                    from 0.00 to 0.00

                                               Greater than zero    All orders whose costs are less than the SP, e.g. from
                                                                    1.00 to 1000


                                           List by
                                           With the selection of the option, you specify how the values of the hit list are
                                           organized:
                                           •   Period
                                               In the Break down by area, you can also resolve the output by Order areas,
                                               Product groups or Orders.
                                               For the evaluation of a year, the data is totaled, e.g. by months. If you have
                                               limited the selection to one month, you can also break down the result by
                                               orders.
                                           •   Product groups:
                                               In the Add up by area, the fields are enabled. In the Break down by area,
                                               the Product group check box is locked.
                                           •   Order areas:
                                               In the Break down by area, you can also resolve the output by Product
                                               groups or Orders.
                                           •   Customers:
                                               In the Break down by area, you can also resolve the output by Order areas,
                                               Product groups or Orders.

                                           Add up by
                                           With the selection of the option, you specify how the values for product groups
                                           should be totaled: The fields are only enabled if you have selected the Product
                                           groups option in the List by area.
                                           •   Main product groups, Product super groups, Product groups:
                                               The values of the period in question are totaled according to the option se-
                                               lected.
                                           •   Top product groups:
                                               The values are totaled according to top product groups. For this, top prod-
                                               uct groups must be created in the master data.
4.01 / 01-2017




                 A+W Business Statistics                                                                                   F-13
                 Sales Statistics                                                             Software Reference




                                    Break down by
                                    With the selection of this option, you specify how the values should be re-
                                    solved. Thus the total quantity is displayed per order area, per product group
                                    or per order.
                                    You can only check one of the check boxes. If you do not check any check box,
                                    the values will be grouped according to the selection criteria.
                                    •   Order areas:
                                        The check box is locked if you have selected the Order areas option in the
                                        Break down by area.
                                    •   Product groups:
                                        The check box is locked if you have selected the Product groups option in
                                        the Break down by area.
                                        If you mark the check box, the Compare with last year’s values check box
                                        in the Options area is enabled.
                                    •   Orders:
                                        The values are sorted by orders.

                                    Options

                                    Compare with last year's values On the tabs, the comparative values for
                                    the previous year can be displayed.
                                     The comparative values are not output.
                                     The comparative values are output. This setting is also taken over in the
                                    default printing.
                                    In sales printing, the comparative values are always displayed.
4.01 / 01-2017




                 F-14                                                                    A+W Business Statistics
                 Software Reference                                                                        Sales Statistics




                                           Order Info – Entered
                                           Statistics > Order info > Entered tab




                                           Fig. F-2     Order info – Entered


                                           This tab displays all orders that were not processed any further. The entry date
                                           is used for selection.
                                           The output can match the output on the Open tab if the selection criteria were
                                           not further limited.
                                           The display of the columns is selected on the Options tab.
                                            “Order Info – Options” on page F-11
4.01 / 01-2017




                 A+W Business Statistics                                                                             F-15
                 Sales Statistics                                                             Software Reference




                                    Order Info – Produced
                                    Statistics > Order info > Produced tab




                                    Fig. F-3     Order info – Produced


                                    This tab displays all orders that were reported finished by production.
                                    The display of the columns is selected on the Options tab.
                                     “Order Info – Options” on page F-11
4.01 / 01-2017




                 F-16                                                                    A+W Business Statistics
                 Software Reference                                                                       Sales Statistics




                                           Order Info – Invoiced
                                           Statistics > Order info > Invoiced tab




                                           Fig. F-4     Order info – Invoiced


                                           This tab displays all orders for which an invoice was written. The invoice date
                                           is used for this.
                                           The display of the columns is selected on the Options tab.
                                            “Order Info – Options” on page F-11
4.01 / 01-2017




                 A+W Business Statistics                                                                             F-17
                 Sales Statistics                                                             Software Reference




                                    Order Info – Open
                                    Statistics > Order info > Open tab




                                    Fig. F-5     Order info – Open


                                    This tab displays all orders that were entered before the current date but not
                                    yet produced. These are all orders for which there is neither an invoice date
                                    nor a batch number.
                                    The display of the columns is selected on the Options tab.
                                     “Order Info – Options” on page F-11
4.01 / 01-2017




                 F-18                                                                    A+W Business Statistics
                 Software Reference                                                                        Sales Statistics




                                           Order Info – Graph
                                           Statistics > Order info > Graph tab




                 Fig. F-6    Order info -- Graph and legend


                                           This tab displays the data of the selection graphically.
                                           The display of the data is selected on the Options tab.
                                            “Order Info – Options” on page F-11

                                           Display
                                           With the selection of the option, you can display the tabs’ data.
4.01 / 01-2017




                 A+W Business Statistics                                                                             F-19
                 Sales Statistics                                                              Software Reference




                                    Selection
                                    Statistics > Order info > Print menu




                                    Fig. F-7     Print setting


                                    On this dialog, you specify how the order information should be output in the
                                    printout.

                                    Select report
                                    With the selection of the option, you specify which tab should be printed.

                                    Select columns (max. 3)
                                    In this area, a check box is displayed for each column from the Open tab. If
                                    you have selected the All option in the Select report area, you can print out a
                                    maximum of three columns.
                                     The column is not printed.
                                     The column is printed.
4.01 / 01-2017




                 F-20                                                                    A+W Business Statistics
                 Software Reference                                                                          Sales Statistics




                                           Turnover Sales
                                           Statistics > Turnover Sales
                                           In addition to printing the turnover information from the Order info dialog, this
                                           dialog also displays detailed evaluations for the sales figures.
                                           This dialog offers the following tabs:
                                           •   “Turnover Sales – Selection” on page F-23
                                           •   “Turnover Sales – Restrictions” on page F-28
                                           •   “Turnover Sales – Table” on page F-29
                                           •   “Turnover Sales – Graph” on page F-30
                                           •   “Turnover Sales – SQL” on page F-31
                                           On the Selection and Restrictions tabs, you specify the criteria for the evalua-
                                           tion of the data.
                                           On the Table and Graph tabs, the result of the evaluation is displayed.


                                           Options menu
                                           Statistics > Turnover Sales
                                           This menu allows you to define the default settings for the dialog. The options
                                           can be enabled or disabled. The settings will not be reset when you close the
                                           dialog.

                                               Activated options after opening the dialog
                                               Please note that changed options only become effective when you open
                                               the dialog.
                                               The following descriptions represent the activated option.

                                           Group settings
                                           •   Quantities incl. BOM:
                                               The quantities from the BOM are included in the specification of the quan-
                                               tity.
                                           •   Only item quantities:
                                               Only the quantity of items is displayed, e.g. 5 pcs. IGU
                                           •   Only BOM quantities:
                                               Only the quantities of the BOM are displayed. This setting is suitable for
                                               processings, for example.
                                           •   Different busin. year active
                                               For annual evaluations, the fiscal year not the calendar year should be re-
                                               garded.
                                           •   Print statistic name:
                                               In the printout, the designation of the statistic should also be specified. The
                                               name is taken from the saved file.
4.01 / 01-2017




                 A+W Business Statistics                                                                                F-21
                 Sales Statistics                                                                Software Reference




                                    Automatic form feed at printing group
                                    •   Following subtotal 1 to 5:
                                        After the selected subtotals, a form feed is inserted into the printout.
                                    •   Before grand total:
                                        A form feed is inserted before the grand total.


                                    Super statistics menu
                                    Statistics > Turnover Sales
                                    You create a super statistic using this menu.
                                    •   Settings:
                                        Opens the Statistics dialog for specifying the super statistic.
                                         “Super Statistics” on page F-32
                                    •   Export, Import:
                                        Opens the dialogs for manual export or import of a super statistic.
                                         “Super Statistics – Export” on page F-34
4.01 / 01-2017




                 F-22                                                                      A+W Business Statistics
                 Software Reference                                                                           Sales Statistics




                                           Turnover Sales – Selection
                                           Statistics > Turnover Sales > Selection tab




                                           Fig. F-8      Turnover sales statistics


                                           On this tab, you specify the criteria for evaluation of the turnover figures. You
                                           can save the settings as a file in order to be able to create equivalent statistics
                                           later on.

                                           Select statistics
                                           If you use particular settings very frequently, you can save them as a file and
                                           select them again.
                                           If you select one of the saved settings again, you must only specify the period
                                           in the Evaluation period area.

                                           Output/totals/sorting

                                           Output The left field lists all output criteria to which the statistical evaluations
                                           can refer.
                                           For the evaluation, you shift all of the output criteria whose values should be
                                           considered.
                                           At least one of the following check boxes must be checked so that data is eval-
                                           uated.
4.01 / 01-2017




                 A+W Business Statistics                                                                                 F-23
                 Sales Statistics                                                                 Software Reference




                                    Create total statistics You can display the total turnover of the company.
                                     Statistics are only formed using the selected criteria.
                                     Statistics are formed using total turnover. This form in particular is useful for
                                    comparative purposes.

                                       Example

                                       If in the Output/totals/sorting area the characteristic Products/Items is
                                       selected, the sales of products is depicted in comparison to the company’s
                                       total sales, e.g. EUR 800,000 vs. EUR 20,000,000.

                                       Performance
                                       This evaluation takes some time since all data for the entire company must
                                       be read in.

                                    Create total selection You can display intermediate totals in the result.
                                     No intermediate total is formed.
                                     The intermediate total is formed per output criterion. For this, the settings
                                    on the Restrictions dialog are considered, e.g. the specified product groups.

                                    Annual evaluation You can summarize the output for an entire year.
                                     The result is not displayed per year. For this setting, you should start a
                                    monthly evaluation.
                                     The result is displayed per year. Considered are the years that are specified
                                    in the Evaluation period area.

                                    Monthly evaluation You can summarize the output per month.
                                     The result is not displayed per month. For this setting, you should start an
                                    annual evaluation.
                                     The result is displayed per month. Considered are the years and months
                                    that are specified in the Evaluation period area.
4.01 / 01-2017




                 F-24                                                                        A+W Business Statistics
                 Software Reference                                                                        Sales Statistics




                                           Direct comparison You can compare the evaluation of several years month
                                           by month.
                                            The evaluation across several years is displayed year by year.
                                            The evaluation across several years is displayed month by month across
                                           the specified years.

                                              Examples for three years and month 1 to 3

                                              Setting           Output

                                                               Year 1         January, February, March
                                                                Year 2         January, February, March
                                                                Year 3         January, February, March

                                                               January        Year 1, Year 2, Year 3
                                                                February       Year 1, Year 2, Year 3
                                                                March          Year 1, Year 2, Year 3


                                           Super statistics You can create statistics as a comparison of the turnover
                                           figures for subsidiaries and/or sites.
                                            No super statistics are created.
                                            The data is created according to the specifications that were made on the
                                           Statistics dialog. No result is displayed on the Table tab.
                                           For a description of this super statistic, see a separate section.
                                            “Super Statistics” on page F-32

                                           Top 10 mode You can limit the statistics to the best results.
                                            The evaluation is not limited to the best results.
                                            In the evaluation, only the best results should be displayed. For this, you
                                           must specify the display of the data in the Top 10 - analysis / sorting area.

                                           Start. month business year For evaluations, the fiscal year not the calen-
                                           dar year should be regarded. The field for entry of the first month is only en-
                                           abled if on the menu Options > Group settings > Different busin. year active
                                           has been activated.
4.01 / 01-2017




                 A+W Business Statistics                                                                             F-25
                 Sales Statistics                                                                 Software Reference




                                    Select categories
                                    With the selection of the categories, you decide which values are output in the
                                    Heading column on the Table tab.

                                        Tip
                                        In the selection of the categories, note that it may cause confusion if you
                                        check too many check boxes. If you need a lot of detail data, create several
                                        statistics with different settings that you save in the Select statistics field
                                        (with a meaningful name).

                                    •   Turnover:
                                        Is displayed in the Heading column as Turnover.
                                    •   Cost calculation:
                                        Is displayed in the Heading column as Costs.
                                    •   Contribution margin:
                                        Is displayed in the Heading column as MI.
                                    •   Contribution margin in %:
                                        Is displayed in the Heading column as CM in %.
                                    •   Average price:
                                        Is displayed in the Heading column as Average price.
                                    •   Turnover in %:
                                        Is displayed in the Heading column as %T.
                                    •   Separate contribution margins:
                                        Is displayed in the Heading column as CM material and CM material %.
                                    •   Pcs.:
                                        Is displayed in the Heading column as Pcs..
                                    •   Area:
                                        Is displayed in the Heading column as Area.
                                    •   Circumference:
                                        Total edge length. Is displayed in the Heading column as Circumference.
                                    •   Weight:
                                        Is displayed in the Heading column as Weight.
                                    •   Turnover complaint:
                                        Only enabled on the Turnover complaint dialog. Is displayed in the Heading
                                        column.
                                    •   Separate costs:
                                        Is displayed in the Heading column as Material cost and Time cost.
                                     The values are not displayed.
                                     The values are displayed.
4.01 / 01-2017




                 F-26                                                                       A+W Business Statistics
                 Software Reference                                                                         Sales Statistics




                                           TOP10 - analysis / sorting
                                           The fields in this area are only enabled if the Top10 mode check box is
                                           checked. In this mode, only the best results are displayed.

                                           Sort by The sort criteria are specified by A+W Software GmbH: CM (contri-
                                           bution margin), area, costs, pieces, circumference, turnover.
                                           With the selection of the option, you specify which value should be listed first.
                                           • Ascending:
                                              For the tops, the highest value is displayed first.
                                           • Descending:
                                              For the flops, the lowest value is displayed first.

                                           Max. lines Number of tops or flops to be evaluated. This way you can limit
                                           the display, e.g. to the 3 tops with the most turnover.
                                           In the table, this is the number of lines. In the graphic, this is the number of
                                           bars.

                                           Evaluation period

                                           Year from, to Year or span of years that should be evaluated.

                                           Month from, to Month or span of months that should be evaluated.

                                           Show amounts

                                           Amounts \ 1000 You can display the monetary units divided by 1000.
                                            The monetary units are displayed unchanged.
                                            The monetary units are displayed divided by 1000. For this setting you
                                           should specify how many places after the decimal point should be displayed.

                                           Digits behind decim. pt. Number of places after the decimal point if the
                                           monetary units are displayed divided by 1000.
4.01 / 01-2017




                 A+W Business Statistics                                                                              F-27
                 Sales Statistics                                                                    Software Reference




                                    Turnover Sales – Restrictions
                                    Statistics > Turnover Sales > Restrictions tab




                                    Fig. F-9      Turnover statistics - Restrictions


                                    On this tab you can limit the evaluations to particular ranges or exclude these
                                    ranges.

                                       Example

                                       Selection tab:                      Restrictions tab:
                                       •   Salesman                        •   Salesman 1
                                       •   Customer group                  •   Customer groups 3-7
                                       •   Business type                   •   Not customer 4000
                                       •   Line of business                •   Products 103 - 106


                                    Select restrictions

                                    Not You can exclude or include the ranges specified in the fields from and to.
                                     The statistics are limited to the specified restrictions.
                                     The specified restrictions are not included in the statistics.

                                    From, to Restriction that should be included in the statistics or excluded
                                    from them.
4.01 / 01-2017




                 F-28                                                                          A+W Business Statistics
                 Software Reference                                                                           Sales Statistics




                                           Minimum turnover for evaluation Specification of the minimum turnover
                                           from which the values in the evaluations should be included.
                                           With the selection of this option you specify whether the specified minimum
                                           turnover should refer to a year or a month.


                                           Turnover Sales – Table
                                           Statistics > Turnover Sales > Table tab




                                           Fig. F-10    Turnover statistics - Table


                                           On this tab, the results of the evaluation are displayed as a table. With the Print
                                           menu you can print the result in tabular form.
4.01 / 01-2017




                 A+W Business Statistics                                                                                F-29
                 Sales Statistics                                                               Software Reference




                                    Turnover Sales – Graph
                                    Statistics > Turnover Sales > Graphic tab




                                    Fig. F-11    Turnover statistics – Graph


                                    This tab displays the data of the evaluation graphically.
4.01 / 01-2017




                 F-30                                                                     A+W Business Statistics
                 Software Reference                                                            Sales Statistics




                                           Turnover Sales – SQL
                                           Statistics > Turnover Sales > SQL tab




                                           Fig. F-12   Turnover statistics – SQL


                                           On this tab, you can create your own SQL queries.
4.01 / 01-2017




                 A+W Business Statistics                                                                 F-31
                 Sales Statistics                                                               Software Reference




                                    Super Statistics
                                    Statistics > Turnover Sales > Super statistics menu > Settings




                                    Fig. F-13    Using group statistics


                                    Use this dialog to export or import the data for the super statistics.

                                    Requirements and goal of super statistics
                                    Super statistics can only be created by main companies and subsidiaries. The
                                    main company/central office and the subsidiaries must be able to communi-
                                    cate with one another via data exchange.
                                    In the super statistics, the sales data of the main company/central office and
                                    the subsidiaries are compared to one another.
                                    The subsidiaries become sites through the assignment to the central office/
                                    main company in a super statistic.
4.01 / 01-2017




                 F-32                                                                      A+W Business Statistics
                 Software Reference                                                                            Sales Statistics




                                                 Central office     Subsidiaries

                                                                                      The following shift takes place:
                                                 Central office 1

                                                 Subsidiary 2       Subsidiary 1      Subsidiary 1            Subsidiary 1
                      Sites                      Subsidiary 3       Subsidiary 2      Subsidiary 2            Subsidiary 2

                                                 Subsidiary 4       Subsidiary 3      Subsidiary 3            Subsidiary 3



                 Fig. F-14    Super statistics


                                            The central office specifies at what intervals the subsidiaries must create and
                                            export ASCII files. All collected subsidiary data is imported into the super sta-
                                            tistics in the central office.
                                            The central office itself can also be a subsidiary and must also export its own
                                            statistics data.

                                            Dialog description

                                            Client ID of the subsidiary or site to which the data is exported.

                                            Statistics Statistics that are created for the data.

                                            Export client ID of the site to which the data is exported. The import system
                                            uses this ID to read in the data for the (target) site.

                                            Import path Directory in which the exported files are located. They are read
                                            in one after another in a loop for the target sites.

                                            Log path Data that cannot be imported is stored in a log file. The administra-
                                            tor must create the missing master data and/or correct the incorrect master da-
                                            ta. On the next import, there is another try to read in the appropriate data
                                            record.

                                            Definition Import
                                            In this area, the importing central office specifies how incoming data should be
                                            booked by default:
                                            • Integration always by default
                                            • Integration 1:1 or by default
                                            • Integration 1:1 compulsory

                                            Standard selection In these fields, you specify the default record in which
                                            the imported data is written.
4.01 / 01-2017




                 A+W Business Statistics                                                                                 F-33
                 Sales Statistics                                                               Software Reference




                                    Super Statistics – Export
                                    Statistics > Turnover Sales > Super statistics menu > Export




                                    Fig. F-15    Super statistics – manual export


                                    On this dialog, you export the ASCII files for the super statistics manually. The
                                    manual export represents an exception in practice. Normally the settings are
                                    made once in the subsidiary, the site number is set, and the rest is done auto-
                                    matically.
                                    Generally the data is also transferred to statistics during the archive transfer:
                                    Documents > Order > Transfer to archive > Sales statistics check box.

                                    Export

                                    Client (local) Site that exports the data.

                                    Select date from, to Specification of the time span in which the file(s) with
                                    the sales data were created.

                                    Overwrite target file There may already be a file with the same name in the
                                    export directory. If you are sure that it has already been incorporated into the
                                    evaluation of the super statistics, you can overwrite the old file.
                                     The old file is not overwritten. The new file distinguishes itself through date
                                    and time stamp.
                                     The old file is overwritten.

                                    Export client ID of the subsidiary or site to which the data is exported, that
                                    is, the target site.

                                    Exported records Number of exported data records in the file.

                                    Export path Path and file name,
                                    e.g. C:\Superstat\Export\0001_20140506.asc.
4.01 / 01-2017




                 F-34                                                                      A+W Business Statistics
                 Software Reference                                                                         Sales Statistics




                                           Super statistics – Import
                                           Statistics > Turnover Sales > Super statistics menu > Import




                                           Fig. F-16    Super statistics – manual import


                                           On this dialog, you import the ASCII files for the super statistics.
                                           The errors encountered are displayed in the system log book and can be iden-
                                           tified using the log files.
                                           Logs are saved with the extension .sav.
4.01 / 01-2017




                 A+W Business Statistics                                                                              F-35
                 Sales Statistics                                                              Software Reference




                                    Complaints Statistics Sales
                                    Statistics > Complaint Sales




                                    Fig. F-17    Complaints statistics sales


                                    On this dialog, you create statistics about complaints in sales. For these sta-
                                    tistics, all documents of the type Complaints are considered.
                                    The fields are described in detail for the Sales Turnover dialog.
                                     “Turnover Sales” on page F-21
                                    For the complaints statistics, you must create a monthly evaluation.
                                    Evaluations of the reason for complaint, cause, and complaint location can
                                    only be created if reasons for complaint and complaint cause are created in
                                    the master data.
4.01 / 01-2017




                 F-36                                                                     A+W Business Statistics
                 Software Reference                                                                         Sales Statistics




                                            Statistics by Structure
                                            Statistics > Statistics by structure
                                            On this dialog, you create evaluations about the structure of lites with BOMs.
                                            Here, only invoiced orders are evaluated.
                                            The result of the evaluation is displayed on the Table tab and can be printed.
                                            This dialog offers the following tabs:
                                            •   “Statistics by Structure – Selection” on page F-37
                                            •   “Statistics by Structure – Table” on page F-40


                                            Statistics by Structure – Selection
                                            Statistics > Statistics by structure > Selection tab




                 Fig. F-18   Statistics by structure – Selection


                                            On this tab, you specify the selection criteria.

                                            Inactivate Lock
                                            You can lock the data records for the duration of the evaluation so that no data
                                            records can be added or changed during the evaluation. This function makes
                                            sense if the evaluation will take a while.
4.01 / 01-2017




                 A+W Business Statistics                                                                               F-37
                 Sales Statistics                                                               Software Reference




                                    Evaluation period

                                    Year, month from, to Specification of the time period that should be evalu-
                                    ated.

                                    Spacer
                                    With the selection of this option, you specify for the evaluation of IG which
                                    spacers should be considered:
                                    •   Total:
                                        All IG lites are evaluated.
                                    •   TPS:
                                        Only IG lites with TPS are evaluated.
                                    •   IG standard:
                                        Only IG lites without TPS are evaluated.

                                    Type
                                    With the selection of this option, you specify the type of products that should
                                    be evaluated:
                                    •   IG:
                                        Only insulated glass is evaluated. With this option, you can also evaluate
                                        IG with additional work.
                                    •   Additional work:
                                        Only additional work is evaluated.
                                    •   Glass types:
                                        Only the glass types are evaluated. The With add. processin check box is
                                        locked.

                                    With add. processin IF you want to evaluate IG, you can also evaluate the
                                    IG with additional processing.
                                     IG lites are evaluated without additional processing.
                                     In addition to the IG lites, IG lites with additional processing are evaluated.

                                    Select restrictions

                                    Salesman from, to Salesmen to whom the evaluation should be limited.

                                    Customer from, to Customers to whom the evaluation should be limited.
4.01 / 01-2017




                 F-38                                                                     A+W Business Statistics
                 Software Reference                                                                         Sales Statistics




                                           Separate by
                                           You can break the evaluation down further. The data is then output, e.g. per
                                           customer and product.
                                            No additional page feed is inserted in the printout.
                                            The additional page feed is inserted in the printout.

                                               Enabled check boxes
                                               • The check boxes Shape, Spacer, Spacer type, and Gas are only en-
                                                 abled if you have selected the type IG.
                                               • The Thickness checkbox is locked if you check the Products check box.

                                           Sort by
                                           With the selection of this option, you specify the sorting of the output:
                                           •   Cust. turnover:
                                               The data is sorted in ascending order per customer by sales.
                                           •   Turnover Cust.:
                                               The data is sorted per customer by sales.
                                           •   Cust. SQM:
                                               The data is sorted in ascending order per customer by area.
                                           •   Cust. structure:
                                               The data is sorted per customer by structure.

                                           Totals

                                           No. of indiv. lines Number of lines after which an intermediate total should
                                           be displayed. If you enter 0, no intermediate totals will be displayed.

                                           Lines in Total Number of lines that should be displayed.

                                           Other

                                           Incl. company total You can display the totals for the participating compa-
                                           nies. On the Table tab, these are the columns Company pieces, Company ar-
                                           ea, Company turnover, Company value/area
                                            The company totals are not displayed.
                                            The company totals are displayed.

                                           Fill columns every time You can suppress the display of names and cus-
                                           tomer number if the selected sorting makes this clearer.
                                            The columns are only filled if the data for the next customer is displayed.
                                            The columns are always filled.

                                           Sep. p. month The totals can be grouped by month.
                                            The totals are displayed chronologically.
                                            The totals are displayed separated by months.
4.01 / 01-2017




                 A+W Business Statistics                                                                               F-39
                 Sales Statistics                                                                        Software Reference




                                             Statistics by Structure – Table
                                             Statistics > Statistics by structure > Table tab




                 Fig. F-19    Statistics by structure – Table


                                             The results of the evaluation are displayed on this tab.
                                             Depending on the filter criteria on the Selection tab, the additional following
                                             columns are displayed:
                                             •   Shape:
                                                 Indication whether shapes are included.
                                             •   Spacer:
                                                 Thickness of the spacer (frame).
                                             •   Spacer type:
                                                 Number of the product group to which the spacer (frame) belongs.
                                             •   Gas:
                                                 Product number of the gas.
                                             By default, the following columns can be displayed:
                                             •   Salesman, Customer:
                                                 If you have not set any limitation in the Selection of restrictions area, the
                                                 names are not displayed.
                                             •   Structure:
                                                 Lite structure, e.g. Float 5 mm + Therm 6 mm if products are displayed or
                                                 4 + 4 + 8 mm if the thickness is displayed.
                                             •
4.01 / 01-2017




                                                 Pcs.:
                                                 Quantity.
                                             •   Area:
                                                 Total area.


                 F-40                                                                               A+W Business Statistics
                 Software Reference                                                                       Sales Statistics




                                           •   Linear m.:
                                               Total edge length.
                                           •   Georgians Type:
                                               Number of grid fields. The number is only displayed if in the Type area the
                                               Insulated glass option is selected.
                                           •   Turnover:
                                               Total sales
                                           •   Surface per unit:
                                               Average area per piece,
                                           •   Value per surface:
                                               Value of the area in local currency, e.g. €/sq m.
                                           •   Value of complaints:
                                               Total value of all complaints per customer in local currency.
                                           •   Value of credit notes:
                                               Total value of all credits per customer in local currency.
                                           •   Qty. Company, SQ/Company, Turnover Company, Amount/surf. Company:
                                               Display of the grand totals. Only displayed if in the Other area the With
                                               company totals check box is checked.
                                           •   Factor:
                                               Ratio of Company value/area to Value per area.
                                           •   Additional work:
                                               Amount of additional work. Only displayed if in the Type area the With ad-
                                               ditional work check box is checked.
4.01 / 01-2017




                 A+W Business Statistics                                                                            F-41
                 Sales Statistics                                                                Software Reference




                                    Customers by Order Area
                                    Statistics > Customers by order area




                                    Fig. F-20     Order areas


                                    On this dialog, you create evaluations of the order areas. You can start the
                                    evaluation across all order areas or limit it to individual ones. The sales values
                                    for the specified year are output per customer and month.

                                    Selection
                                    With the selection of the option, you specify which order areas should be re-
                                    garded.
                                    •   Select order areas:
                                        The Select order areas area is enabled. The statistics are created for all or-
                                        der areas that are marked in this selection.
                                    •   All order areas with turnover:
                                        The statistics are created for all order areas in which turnover was found.
                                        The Select order areas area is locked.

                                    Year Year that should be regarded.
4.01 / 01-2017




                 F-42                                                                      A+W Business Statistics
                 Software Reference                                                                          Sales Statistics




                                           Printout mode
                                           With the selection of the option, you specify whether the statistics should be
                                           output on the screen or on a printer.

                                           Select order areas
                                           This area lists all order areas. The selection is only enabled if the Select order
                                           areas option is selected. The statistic is created for all order areas whose
                                           check boxes are checked.
4.01 / 01-2017




                 A+W Business Statistics                                                                               F-43
                 Purchasing Statistics                                                              Software Reference




                                         Purchasing Statistics
                                         In addition to the sales information, there are also detailed evaluations avail-
                                         able for purchasing figures.
                                         This chapter provides information on the following subjects:
                                         •   “Turnover Purchase Statistics” on page F-44
                                         •   “Complaint Purchase Statistics” on page F-45
                                         •   “Delivery Date Compliance” on page F-46
                                         •   “Consumption Analysis” on page F-48


                                         Turnover Purchase Statistics
                                         Statistics > Turnover Purchase




                                         Fig. F-21    Turnover purchase statistics


                                         On this dialog you create statistics about purchasing. For this, the purchase
                                         orders are evaluated.
                                         The fields are described in detail for the Turnover Sales dialog.
                                          “Turnover Sales” on page F-21
4.01 / 01-2017




                 F-44                                                                          A+W Business Statistics
                 Software Reference                                                                  Purchasing Statistics




                                           Complaint Purchase Statistics
                                           Statistics > Complaint Purchase




                                           Fig. F-22    Complaint purchase statistics


                                           On this dialog, you create statistics about complaints in purchasing. All in-
                                           voiced purchase orders are considered for these statistics.
                                           The fields are described in detail for the Turnover Sales dialog.
                                            “Turnover Sales” on page F-21
4.01 / 01-2017




                 A+W Business Statistics                                                                              F-45
                 Purchasing Statistics                                                                Software Reference




                                          Delivery Date Compliance
                                          Statistics > Del. date compliance




                 Fig. F-23   Del. date compliance


                                          On this dialog you create statistics about the delays that have occurred for de-
                                          liveries or orders. The date shifts are considered for the evaluation.

                                          Selection

                                          Mode With the selection of the option, you specify according to which part-
                                          ners the evaluation should be done:
                                          • Customers:
                                             The delivery date shifts are evaluated. These shifts can be caused by, e.g.,
                                             delayed deliveries of purchased parts or production dates.
                                          • Suppliers:
                                             Delayed deliveries due to the suppliers are evaluated.

                                          Database With the selection of the option, you specify what data scope
                                          should be evaluated:
                                          • Main database + current archives:
                                             The main database and the current archive year are evaluated.
                                          • Archives year:
                                             Only a particular archive is evaluated. The field for selection of the archive
                                             is enabled. With this setting, no documents can be considered that are in
                                             the main database.
4.01 / 01-2017




                 F-46                                                                            A+W Business Statistics
                 Software Reference                                                                 Purchasing Statistics




                                           Restrictions

                                           Period from, to Time period that should be evaluated.

                                           Evaluation limit 1, 2 Number of delay days. With the selection, the display
                                           in the table columns changes.

                                           From customer no., to Customer or sequence of customers for which de-
                                           lays should be evaluated.

                                           Customer group Customer group that should be evaluated for the delays.

                                           Do not limit All customers should be evaluated.

                                           Table
                                           In the overview, the result of the evaluation is displayed per customer or sup-
                                           plier.
                                           • Ø Days earlier, Ø Days later:
                                             Average of both evaluation limits in days.
                                           • > n Days Earlier:
                                             Number of orders per evaluation limit that are over the limit.
                                             For suppliers, these are the purchase orders that were over the limit.
                                           • < n Days Later:
                                             Number of orders per evaluation limit that are below the limit.
                                           • In Time:
                                             Number of orders that were delivered on the agreed-upon date.
                                           The display closes with a total line.
4.01 / 01-2017




                 A+W Business Statistics                                                                            F-47
                 Purchasing Statistics                                                                 Software Reference




                                          Consumption Analysis
                                          Statistics > Consumption analysis
                                          You can evaluate the material consumption according to criteria you select.
                                          This dialog offers the following tabs:
                                          •   “Consumption Analysis – Selection” on page F-48
                                          •   “Consumption Analysis – Restrictions” on page F-51
                                          •   “Consumption Analysis – Table” on page F-53

                                          Options menu
                                          •   Automatic page feed active:
                                              A page feed is inserted in the printout automatically.


                                          Consumption Analysis – Selection
                                          Statistics > Consumption analysis > Selection tab




                 Fig. F-24   Consumption analysis – Selection


                                          On this tab, you specify the criteria for the evaluation.
4.01 / 01-2017




                 F-48                                                                            A+W Business Statistics
                 Software Reference                                                                   Purchasing Statistics




                                           Source

                                           Number Order that should be evaluated.

                                           Archives The archives can be included in the search for an individual order.
                                            There is a search for the order only in the main database.
                                            There is a search for the order in the main database and in the archives.

                                           Number Manager Selection of the number manager. With this option, the
                                           fields in the Evaluation period area are locked.

                                           Client Site to which the evaluation should be limited.

                                           Order area Order area to which the evaluation should be limited.

                                           Evaluation period
                                           The fields in this area are locked if the Number Manager option is selected.

                                           By delivery date from, to Time period of delivery dates that should be eval-
                                           uated.

                                           By production date from, to Time period of production dates that should
                                           be evaluated.

                                           Select status area

                                           From, to Status range of the documents that should be evaluated.

                                           Select product

                                           Product type Product type that should be evaluated. You can delete the de-
                                           fault selection <k.A.>.

                                           Product class Product class that should be evaluated.

                                           Articles Product that should be evaluated.

                                           Sequence/total calculation
                                           You can specify according to which criteria the results should be sorted. A total
                                           is formed per criterion selected.

                                           Selection fields The criteria selected are displayed in the right field and can
                                           be shifted into the desired sequence using the arrow keys.
4.01 / 01-2017




                 A+W Business Statistics                                                                              F-49
                 Purchasing Statistics                                                               Software Reference




                                         Break down per order The result can be displayed in detail by order.
                                          One line is displayed per sort criterion.
                                          One line is displayed per sort criterion and order.

                                         Break down per item The result can be displayed in detail by items.
                                          One line is displayed per sort criterion. If the breakdown is by order, the or-
                                         der items are not listed individually.
                                          One line is displayed per sort criterion and order item.

                                         Selection product areas
                                         You can limit the statistics to individual product areas of the following glass
                                         types: Single annea (simple glass), TG, LG, IG.
                                          The data from this product area is not output in the statistics.
                                          The data from this product area is output in the statistics.

                                         Options

                                         Related gas calcul. Not currently used.

                                         Quantity unit Quantity unit in which the gas should be specified.
4.01 / 01-2017




                 F-50                                                                           A+W Business Statistics
                 Software Reference                                                                  Purchasing Statistics




                                           Consumption Analysis – Restrictions
                                           Statistics > Consumption analysis > Restrictions tab




                 Fig. F-25   Consumption analysis – Restrictions


                                           On this tab you can further limit the selection of the analysis by consumption.

                                           Source
                                           With the selection of the option, you specify which documents should be eval-
                                           uated:
                                           •   Number:
                                               An individual order should be evaluated. The field for input of the order
                                               number and the Archive check box are enabled.
                                           •   Number Manager:
                                               The orders of a number manager should be evaluated.

                                           Archives The specified document can also be searched for in the archive.
                                            There is no search in the archives.
                                            The document should be searched for in the archive if it is not found in the
                                           main database. This setting makes sense if you archive documents in short
                                           periods.

                                           Client Site to which the evaluation should be limited.

                                           Order area Order area that should be evaluated.
4.01 / 01-2017




                 A+W Business Statistics                                                                             F-51
                 Purchasing Statistics                                                              Software Reference




                                         Evaluation period
                                         With the selection of the option, you specify from which time period documents
                                         should be evaluated:
                                         •   By delivery date:
                                             The specified period refers to the delivery date.
                                         •   By production date:
                                             The specified period refers to the date on which production was started.

                                         From, to Time period that should be evaluated.

                                         Select status area

                                         From, to Status range of the documents that should be evaluated.

                                         Select product

                                         Product type Product type that should be evaluated.

                                         Product class Product class that should be evaluated.

                                         Articles Product that should be evaluated.

                                         Selection supply types
                                         The evaluation can also be limited to procurement types.
                                          The procurement type is not considered.
                                          Only products with this procurement type should be evaluated.

                                         Selection product types
                                         The evaluation can also be limited to product types.
                                          The product type is not considered.
                                          Only products of this product type should be evaluated.
4.01 / 01-2017




                 F-52                                                                           A+W Business Statistics
                 Software Reference                                                                  Purchasing Statistics




                                           Consumption Analysis – Table
                                           Statistics > Consumption analysis > Table tab




                 Fig. F-26   Consumption analysis – Table


                                           The results of the evaluation are displayed on this tab. The display of the col-
                                           umns and rows depends on the settings that you have specified on the Selec-
                                           tion tab.
4.01 / 01-2017




                 A+W Business Statistics                                                                             F-53
                 Commission Statistics                                                              Software Reference




                                          Commission Statistics
                                          Statistics > Commission statistics




                 Fig. F-27   Commission statistics


                                          On this dialog, you evaluate the salesmen's commissions.

                                          Selection

                                          Salesman Salesman if the evaluation should be limited to an individual
                                          salesman.

                                          From, to Time period that should be evaluated.
                                          With the selection of the option, you specify the period to which reference is
                                          made.
                                          • By invoice date:
                                             With this setting you only evaluate invoiced documents.
                                          • By entry date:
                                             With this setting you evaluate all documents in the specified period.
                                          • By transfer date:
                                             With this setting you evaluate documents that were transferred to the sta-
                                             tistics in the specified period.
4.01 / 01-2017




                 F-54                                                                          A+W Business Statistics
                 Software Reference                                                              Commission Statistics




                                           Subtotal
                                           You can set whether and where subtotals should be formed.

                                           Per representative If you evaluate the documents for all representatives,
                                           you can form one subtotal per representative.
                                            No subtotals are formed. This setting makes sense if you create the evalu-
                                           ation for a particular representative.
                                            A subtotal is inserted after each representative.

                                           Per customer If you evaluate the documents across a longer time period,
                                           you can form one subtotal per customer.
                                            No subtotals are formed.
                                            A subtotal is inserted per customer.

                                           Result
                                           The overview displays the following columns:
                                           •   Represent.:
                                               Name of the representative.
                                           •   Invoice no., Invoice date:
                                               Number and date of the invoice.
                                           •   Order no.:
                                               Order number.
                                           •   Input date:
                                               Entry date.
                                           •   Total turnover:
                                               Grand total of the order.
                                           •   % Commission:
                                               Commission rate in the order.
                                           •   Total commission:
                                               Amount of the commission.
                                           •   Customer ID, Name Customer:
                                               Number and name of the customer.
                                           •   Transfer date:
                                               Transfer to statistics.
                                           •   Country:
                                               Country in which the customer is located.
4.01 / 01-2017




                 A+W Business Statistics                                                                         F-55
                 Intrastat Message                                                                 Software Reference




                                          Intrastat Message
                                          Statistics > Intrastat Message




                 Fig. F-28   Intrastat message


                                          On this dialog, you create evaluations of the Intrastat messages.

                                          Identification

                                          Client Site for whose documents the statistics are created.

                                          Employee Employee logged in.

                                          Order NM Number manager in which the orders are collected.

                                          Credit note NM Number manager in which the credits are collected.

                                          Default

                                          Archives Archive whose documents should be evaluated.
4.01 / 01-2017




                 F-56                                                                         A+W Business Statistics
                 Software Reference                                                                   Intrastat Message




                                           Create new NM
                                           The fields in this area are only enabled if you create a new number manager.
                                           To do this, select menu Start > [New].

                                           Invoice date to, from Time period in which the orders were invoiced.

                                           Country code Country for which you want to create the statistics. Only the
                                           country codes are available for selection that are stored in the master data.

                                           Name of order NM Entry of the name. Select a meaningful name so that you
                                           can recognize which documents are collected in this number manager.

                                           Name of credit note NM Entry of the name. Select a meaningful name so
                                           that you can recognize which credits are collected in this number manager.

                                           Documents to be reported
                                           The overview displays all documents that are collected in the selected number
                                           manager.
                                           •   PCH Country:
                                               Country from which the goods were imported.
                                           •   Number:
                                               Order number.
                                           •   P.O. number:
                                               Purchase order number.
                                           •   OC supplier:
                                               Number of the order confirmation by the supplier.
                                           •   Invoice:
                                               Invoice number for the customer order.
                                           •   Date Del. date:
                                               Number of the delivery by the supplier.
                                           •   Order number:
                                               Order number.
                                           •   Shipping date:
                                               Delivery date from the factory.
                                           •   Customer/supplier:
                                               Customer or supplier number.
                                           •   Name, Matchcode:
                                               Name and match code of the customer or supplier.
                                           •   Status:
                                               Document status.
                                           •   Date Entry:
                                               Entry date of the document.
                                           •   OC date:
                                               Date of the order confirmation.
                                           •   Prod. Date IG, LG, TG:
                                               Production date for the glass type.
4.01 / 01-2017




                                           •   Batch no. Prod. IG, LG, TG:
                                               Number of the production batch.



                 A+W Business Statistics                                                                           F-57
                 Intrastat Message                                                             Software Reference




                                     •   Delivery date:
                                         Delivery date to the customer.
                                     •   Delivery note:
                                         Delivery note number.
                                     •   Date of delivery:
                                         Delivery date.
                                     •   Invoice, Invoice date:
                                         Number and date of the invoice.
                                     •   Total quantity:
                                         Total quantity.
                                     •   Sq m real:
                                         Total area.
                                     •   Lin. M real:
                                         Actual linear meters of the edge length.
                                     •   Total weight:
                                         Total weight.
                                     •   Sq m invoiced:
                                         Total area invoiced.
                                     •   Lin m. invoiced:
                                         Edge length invoiced.
                                     •   Net amount:
                                         Net invoice amount.
                                     •   Route:
                                         Name of the delivery route.
                                     •   Business type:
                                         Designation of the business type.
                                     •   Order area:
                                         Designation of the order area.
                                     •   Representative 1, Representative 2:
                                         Name of the participating representative.
                                     •   Lock ID:
                                         Lock ID from the additional information about the order.
4.01 / 01-2017




                 F-58                                                                     A+W Business Statistics
Statistics               F

                  Part index




             A+W Business
                 Part index                                                                     Index




                 Index
                 A                                         Order Information F-10
                 Analysis                                  – Entered F-15
                 – Consumption        F-48                 – Graph F-19
                                                           – Invoiced F-17
                                                           – Open F-18
                 C
                                                           – Options F-11
                 Commission
                                                           – Print setting F-20
                 – Statistics F-54
                                                           – Produced F-16
                 – Statistics by salesmen F-54
                                                           Overview
                 Compare with last year's values    F-14
                                                           – Invoiced orders F-17
                 Complaints statistics
                                                           – Open orders F-18
                 – Purchasing F-45
                                                           – Orders entered F-15
                 – Sales F-36
                                                           – Produced orders F-16
                 Consumption
                 – Analysis F-48
                 Consumption analysis                      P
                 – Restrictions F-51                       Print
                 – Result F-53                             – Order info F-20
                 Customers                                 Purchasing
                 – By order areas F-42                     – Complaints statistics   F-45
                                                           – Turnover F-44
                 D
                 Del. date compliance        F-46          R
                                                           Restrictions
                                                           – Consumption analysis F-51
                 E
                                                           – Turnover SP, PP F-28
                 Export
                                                           Result
                 – Super statistics    F-34
                                                           – Consumption analysis F-53

                 G                                         S
                 Graph
                                                           Sales
                 – Order info F-19
                                                           – Complaints statistics F-36
                 – Turnover SP, PP F-30
                                                           – Graph F-30
                 – Turnover statistics F-30
                                                           – Turnover F-21
                                                           Selection
                 I                                         – Consumption analysis F-48
                 Import                                    – Rubrics in sales statistics F-26
                 – Super statistics    F-35                – Turnover SP, PP F-23
                                                           Setting
                 L                                         – Super statistics F-32
                 List by   F-13                            Show amounts F-27
                                                           SQL
                                                           – Turnover SP, PP F-31
                 O
                                                           Statistics
                 Options
                                                           – Del. date compliance F-46
                 – Order info F-11
                                                           – Turnover SP, PP F-29
4.01 / 01-2017




                 Order area
                 – Customer statistics       F-42




                 A+W Business Statistics                                                        F-61
                 Index                                             Part index




                 Structure
                 – Result of the statistics F-40
                 – Selection of the statistics F-37
                 – Statistics F-37
                 Super statistics
                 – Export F-34
                 – Goal, requirement F-32
                 – Import F-35
                 – Menu F-22
                 – Settings F-32

                 T
                 TOP 10 statistics F-25
                 – Analysis, sorting F-27
                 Turnover
                 – Graph F-30
                 – Output, totals, sorting F-23
                 – Purchasing F-44
                 – Restrictions F-28
                 – Result F-29
                 – Sales F-21
                 – Selection F-23
                 – SQL query F-31
4.01 / 01-2017




                 F-62                                 A+W Business Statistics

