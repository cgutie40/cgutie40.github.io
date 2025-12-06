---
title: Hardware V2.0
tags:
- tag1
- tag2
---
### PCB Revision Plan: Footprint, Testability, Gain and Protection

I want to shrink the PCB footprint. The board is about **100 × 100 mm** now and still feels bulky despite some unused areas. Reorganizing components and tightening the layout should cut size and make the board easier to carry.

I will add a dedicated test point to the ground plane since the current design only exposes top layer test points. That will simplify debugging and give more reliable reference measurements.

Functionally, I plan to rework the gain stage. The sensor’s current output sits in a higher than expected voltage window, which leaves only a narrow range to trigger the alarm. Reducing the amplifier gain or shifting the window will widen the usable range and make sensitivity adjustments more effective across different humidity conditions.

Finally, I want basic protection around the sensor and vulnerable PCB areas. A full enclosure would be ideal, but a protective mesh or conformal coating over the board could be a lower cost way to guard against dust and moisture while keeping access for testing.
