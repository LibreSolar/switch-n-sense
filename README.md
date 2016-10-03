# Switch-N-Sense
High-side NMOS power switch and current sense resistor for battery applications

This device is the power part of the new generation Libre Solar 24V-48V BMS, but can also be used for lead-acid battery protection switches.

The connector to the BMS (IDC connector) is placed at the same height as in the BMS PCB. So mount this PCB right next to the BMS PCB (right side).

## Design considerations

The MOSFETs and the sense resistors are mounted at the back side of the PCB and should be attached to a large heat sink via thermal interface materials (e.g. thermal pad).

[Würth Power Elements WP-BUCF (order code 7461059)](https://powerelement.we-online.de/p/s/1406/93172-PowerOne-Bush-vertical-through-hole.html) are used for wire to board connection.

## Current target

Current rating can be adjusted depending on chosen MOSFETs and sense resistors.

- Maximum number of MOSFETs: 2 in parallel
- Maximum number of sense resitors (2512): 4

Targets for fully populated PCB (total heat dissipation approx. 20 W in MOSFETs, connectors and sense resistor at full current):

| MOSFET (2x) | Voltage | Maximum Current | Remark                                       |
|-------------|---------|-----------------|----------------------------------------------|
| FDMT80080DC | 48V     | 80 A            |                                              |
| FDMT80060DC | 12V/24V | 100 A           |                                              |
| CSD18540Q5B | 12V/24V | 60 A            | cheap alternative, but needs other footprint |
