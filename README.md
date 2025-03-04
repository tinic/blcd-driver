# blcd-driver
Motor driver for brushless air conditioner motors

This is a PCB design for typical adjustable brushless motors used in air conditioning units. These units are great since they are sealed and have ajustable speed while using very little power. I used them to drive a stirrer motor to replace the misspecced AC motors in KOMOS KRYO Inline Draft Beer Chillers which tend to fail quickly and generate extreme amounts of heat. Power consumption is reduced from ~17W to around ~4W for my application.

The following units have been tested:

140VDC rated (on 120VAC power):
- ZKFP-20-8-113

310VDC rated (on 240VAC power):
- WZDK30-38G

While these units are rated 140/310VDC they work fine with regular rectified AC power (170/338VDC) which makes the implementation simple/cheap.

![Alt text](ac-dc-converter.png)
