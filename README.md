# VOR Parts Tracker

`vor-parts-tracker.html` is a single file. Open it in a browser and upload the depot's Parts VOR Log (.xlsx).

- **Tab 1, Parts:** Date Requested, Date Ordered, Bus Number, Part Number, Part Description, Comments, Date Due, Date Arrived
- **Tab 2, Buses:** Date, Bus Numbers on Log (comma separated, e.g. `12345, 12343MOT, 12121`)

Buses entered with **MOT** after the number (`12343MOT`, `12343 MOT` or `MOT 12343`) go in their own MOT section. They are left out of the VOR awaiting / not-awaiting figures.

A bus counts as off road from the first logged day it appears until the first logged day it is missing. Parts are linked to a VOR spell by bus number and request date (up to 7 days before the bus came off road).
A bus is "awaiting parts" on a day when it is off road and has a linked part that has been requested but has not arrived.

Exports: **PDF report** (KPIs, daily trend, Gantt, parts log, history) and a **standalone HTML** snapshot with the data embedded.
