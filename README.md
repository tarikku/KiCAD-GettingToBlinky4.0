# KiCAD-GettingToBlinky4.0
The PCB I made following Chris Gammell's KiCAD 4.0 tutorial - Getting To Blinky 4.0 (https://www.youtube.com/playlist?list=PLy2022BX6Eso532xqrUxDT1u2p4VVsg-q).

I used the most recent version of KiCAD (5.0) to create the PCB. The main difference I encountered, as identified by the DRC, was that the battery holder footprint did not include a courtyard. This seems not to have been checked in KiCAD 4.0.

KiCAD 5.0 requires all parts to have a defined courtyard, i.e. rectangular area around the part providing enough electrical and mechanical clearance (http://kicad-pcb.org/libraries/klc/F5.3/)
There are special layers within the part's footprint for this that need to be filled (Front and/or Back courtyard layer). After having filled in the Front courtyard layer with an outline of the part, the DRC was happy.
