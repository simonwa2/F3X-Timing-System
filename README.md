# F3X Timing System

## About

## News

### 1 June 2019
**Uni-Timer Version 1.0.3 released.**  It contains the ability to save credentials for multiple wifi access points to allow easy switching, and also adjustable auto restart delay for practice flights:

http://github.com/simonwa2/F3X-Timing-System/tree/master/Uni-Timer/Firmware/Version%201.0.3

**Bluetooth Audio option being evaulated.**  Sends audio to a bluetooth speaker.  Tested successfully with a new version of the Uni-Timer circuit board, but it requires that the speaker supports Bluetooth 5.  It should also be able to be retrofitted to older Uni-timer and CD units.   

## Timing system Units

### CD Unit
Used to time and manage contests (pilots, rounds, flights). 
Provides announcements for countdowns, turn signals and flight time. 
Works with f3xvault (via wifi) for data download and upload.  Has
anemometer integration for wind speed and direction. Links to base,
audio and wind units for completely wireless operation.  Uses a high
brightness colour touchscreen for operation.  As well as piCAMTracker,
it also works with MotCam.

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/CD_unit_small.jpg" width="256" title="CD Unit">

### Uni-Timer
Cutdown version of CD unit.  Provides announcements for
countdowns, turn signals and flight time.  Links to base units for
completely wireless operation (and audioand wind in the near future). 
But (at the moment) does not manage contests and does not link to
f3xvault.  Only has a small screen, but provides web pages for extending
capability to smart phones.  Also much cheaper than CD Unit.  It was
originaly intended to be only used for training (particularly with
piCAMTracker), but now my intention is to extend it to full contest
management as well.

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/unitimer1.jpg" width="256" title="UniTimer">

### Repeater
Range extender for the local network that links the units.  Placed on a pole near the centre of the course.   Only necessary where the terrain is hilly and the bases do not have clear line of sight of the course center.

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/repeater_small.jpg" width="90" title="Repeater">

### Coordinator
Now replaced by the Repeater.  Manages the local  network and acts as a range extender for the local network that links the units. 
### Base
Now replaced by UniTimer. Wireless base button with flight data display.
### Wind
Will be replaced by UniTimer. Wireless transfer of anemometer data to CD or UNiTimer units.
### Audio
Will be replaced by UniTimer.  Wireless audio with line out for connecting to a powered speaker.
### Display
Wireless large panel LED display for showing flight data to other pilots and watchers. 400mm x 400mm high brightness colour display.
### Team
The Team unit is designed primarily for F3B.  It provides flight data to support the distance and duration tasks. It can also act as Base A - reducing the number of people required to run the distance task.  The unit also works as a basic F3F timer (no data storage).

## Supported Camera Systems

* Motcam
* piCAMTracker
