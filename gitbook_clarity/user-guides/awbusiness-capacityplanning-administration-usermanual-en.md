---
description: "EN-UM-AWBusiness_31"
---


# Software Reference

---
## Administration

are logged if no booking is made in the capacity planning.
The history can be evaluated in the Statistics module and printed out.

### Automatic delivery date search by route
In case of bottlenecks, it is possible to search for a new delivery date automatically.
- [ ] The next possible date is selected as delivery date regardless of whether it is a route day or not. This is the default setting.
- [ ] The program searches for a new delivery date based on the customer's route days.

### Do not split order
Large orders must be split into smaller items if the work process cannot be performed completely for an order in one day.
- [ ] The orders can be split for automatic scheduling. This is the default setting.
- [ ] The orders can only be split manually. For the automatic scheduling of large orders, a message is displayed so that you can intervene.

### Reduced scheduling check if structure identical
An order may contain items with the same BOM structure, which differ only according to the dimensions.
- [ ] The entire BOM structure is checked for each item.
- [x] With the same BOM structure, the scheduling assumes the previous item without checking the BOM. This is the default setting.

### Schedule for delivery date
For automatic scheduling, orders are scheduled for the delivery date by default. Only if no capacities are free is another delivery date sought.
- [ ] Orders are scheduled with delivery date search. This is the default setting.
- [ ] The orders are scheduled without a search for an alternative delivery date, regardless of whether or not capacities are free.

### Automatic completion report for invoiced orders
Currently not used.

### Transfer to production (OrderXML) incl. planning data
For the transfer to production, the data determined from capacity planning can be written into the OrderXML file.
- [ ] The data determined from capacity planning is not written into the OrderXML file.
- [ ] The machine allocation, production date and shift, time costs are written to the transfer file.

### Use change of shifts table
If you work with more than one shift, you can specify when the scheduling changes from one shift to the next.
- [ ] The change of shifts table is not used.
- [ ] The change of shifts table is used. If no shift changes are specified, the Shift settings dialog opens.
⇨ "Shift settings" on page H-2837

### Product classes without status change
You can suppress the increasing of the item status (order status) with completion reports for product classes. Just select the appropriate entries on the list.

### WP areas without scheduling
⇨You can specify that in particular WP areas, there is no automatic scheduling. This means that orders for the marked WP areas can only be scheduled manually.

### Shift settings
**Path:** Master data > Company > Company data > Capacity planning tab > Use change of shifts table checkbox

