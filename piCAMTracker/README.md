# Introduction

piCAMTracker is a Raspberry Pi camera based crossing detection system developed by Axel (Barney) Barnitzke.  Details of the system are available here:

https://github.com/barney-NG/piCAMTracker

To connect piCAMTracker to the timing system, a plug-in board (pi hat) was developed.  The board provides the radio link and also power management for the Raspberry Pi.  Details are on Barney's GitHub pages here:
here:

https://github.com/barney-NG/piCAMTracker/wiki/PCB-Hat

# Details

## Power Management
The board uses a switching regulator to provide 5V to the Raspberry Pi.  The input voltage can be between 6V and 36V.  Three 18650 Li Ion batteries in a 3S configuration works well.
A slide switch controls power.  When switched to The Off position, a signal is sent to the Raspberry Pi to do a safe shutdown.  Power is removed several seconds later.

## Radio Link
An Xbee radio module is used for the 2.4GHz link to the timing system.  The link is bi-directional and allows the timing system to query the unit for useful data such as battery voltage and signal strength.

## Turn signalling
Two turn signals are sent:
* piCAMTracker Turn signal
* External switch.  An external switch can be connected to the CMD3 and GND pads on the expansion port.

## Expansion Port
The expansion port provides the following signals:
* +3.3V
* GND
* CMD1 (Input)
* CMD2 (Input)
* CMD3 (Input) used for external switch and sent to timing system by Xbee
* TURN (Output) from piCAMTracker)
* CUT (Output) from piCAMTracker)

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/CD_unit_small.jpg" width="256" title="picam_piHat">

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/CD_unit_small.jpg" width="256" title="picam_battery">
