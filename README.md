# F3X Timing System

## About
The F3X Timing System is a wireless solution for F3F and F3B.  It has been developed and evolved over many years, primarily in response to a need to simplify event timing and management in Western Australia.  In recent years systems have been built for individuals and clubs outside of Australia.

### Simple System for Training Example
<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/UniTimer_no_wifi1.png" width="768" title="F3F">

### Full System Example
<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/f3f_network_1.jpg" width="1024" title="F3F">

***
## News

### 19 January 2021
**Transition to ESP NOW radio link.**  Development of a new radio link between modules is nearing completion.  It utilises the ESP NOW protocol available on ESP8266 and ESP32 processors.  ESP NOW provides significantly lower latency and hardware cost than the Xbee modules that the timing system has used for many years.
Existing timing system units will be able to be upgraded to ESP NOW via a plug-in module that replaces the Xbee.  New units have also been developed that utilise ESP NOW.

A short video demonstrating the system is available :
https://www.youtube.com/watch?v=c-oyRrp0d6k&feature=emb_logo

The video also shows the new UniTimer V2 which is a major upgrade from the original UniTimer with an improved and larger display.

Upgrade modules and new units will available from March 2021 (subject to successful contest testing of ESP NOW in February).

### 18 November 2019
**CD Unit Version 2.7 released.**  Support for creating offline events and adding pilots, auto-restart options for practice flights, flight times > 99 secs, mark pilot as out of round or event, various fixes:

https://github.com/simonwa2/F3X-Timing-System/tree/master/CD%20Unit/Firmware/Version%202.7

### 26 July 2019
**Uni-Timer Version 1.0.6 released.**  Improved legibility of startup screen, fixed issue with Practice Laps mode:
https://github.com/simonwa2/F3X-Timing-System/tree/master/Uni-Timer/Firmware/Version%201.0.6

### 19 July 2019
**Uni-Timer Version 1.0.5 released.**  It improves the bluetooth button reliablity and reduces latency in the audio:
https://github.com/simonwa2/F3X-Timing-System/tree/master/Uni-Timer/Firmware/Version%201.0.5

Bluetooth audio has now been added. A small bluetooth transmitter module sits in the case.  A Bluetooth speaker can be paired to it.  Although suitable for practice, standard bluetooth audio has too much inherent latency for contest use. 

***
## Timing system Units

### CD Unit
Used to time and manage contests (pilots, rounds, flights). 
Provides announcements for countdowns, turn signals and flight time. 
Works with f3xvault (via wifi) for data download and upload.  Has
anemometer integration for wind speed and direction. Links to base,
audio and wind units for completely wireless operation.  Uses a high
brightness colour touchscreen for operation.  As well as piCAMTracker,
it also works with MotCam.

Key Features:
* Size: approx 180mm x 85mm x 34mm
* Weight: about 400g
* Power: 2 x 18650 batteries (removeable).
* Display: 4.5 inch high intensity colour touchscreen
* 2.4GHz local network (xbee) for connectivity to external units such as base units or piCAMTracker 

Timing functions:
* flight timer - displayed and announced flight states, countdowns, turn beeps and count, flight time announcement at the end
* lap timer - displayed and announced turn beeps and lap times
Event functions:
* integration with F3XVault - search and download events and upload flight data
* create rounds - set flight order
* run the flights
* all flight data saved to sd card
Anemometer support:
* direct connect David or Peet Bros anemometers or connect to Wind unit for wireless wind data
Compatibility with camera systems:
* MotCam (with F3X Base unit)
* piCAMTracker (with the pi hat)
Audio:
* line out to connect to powered speaker or wireless conenction to Audio unit
Firmware updates:
* by usb upload and sd card

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

Key Features:
* Size: approx 100mm x 60mm x 30mm
* Weight: about 120g
* Power: built in LiPo with USB charging. Expected to last at least 8 hrs between charges.
* Display: 0.9 inch - not very big but high resolution so easy to read
* 2.4GHz local network (xbee) for connectivity to external units such as base units or piCAMTracker (same as the existing fleet of timing units)

Timing functions (initial set):
* flight timer - displayed and announced flight states, countdowns, turn beeps and count, flight time announcement at the end
* lap timer - displayed and announced turn beeps and lap times
Compatibility with camera systems:
* MotCam (with F3X Base unit)
* piCAMTracker (with the pi hat)
Audio:
* line out to connect to powered speaker or a bluetooth transmitter
Wifi:
* either connect to an existing wifi access point, or run it's own wifi
* provides web page for access to setup menu and flight data/control from smartphone or tablet
Bluetooth:
* Remote bluetooth button (ITAG) for pilot control of unit (e.g. flight start/reset)
Firmware updates:
* by web interface


<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/unitimer1.jpg" width="256" title="UniTimer">

### Repeater
Range extender for the local network that links the units.  Placed on a pole near the centre of the course.   Only necessary where the terrain is hilly and the bases do not have clear line of sight of the course center.

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/repeater_small.jpg" width="90" title="Repeater">

### Coordinator
Now replaced by the Repeater.  Manages the local  network and acts as a range extender for the local network that links the units. 
### Base
Now replaced by UniTimer. Wireless base button with flight data display.

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/base_unit_v1.jpg" width="200" title="Base">

### Wind
Will be replaced by UniTimer. Wireless transfer of anemometer data to CD or UNiTimer units.

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/wind_unit.jpg" width="200" title="Wind">

### Audio
Will be replaced by UniTimer.  Wireless audio with line out for connecting to a powered speaker.
### Display
Wireless large panel LED display for showing flight data to other pilots and watchers. 400mm x 400mm high brightness colour display.

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/display_unit_1.jpg" width="256" title="Display">

### Team
The Team unit is designed primarily for F3B.  It provides flight data to support the distance and duration tasks. It can also act as Base A - reducing the number of people required to run the distance task.  The unit also works as a basic F3F timer (no data storage).

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/team_and_base_coord.jpg" width="256" title="Team">


## Supported Camera Systems

* Motcam
* piCAMTracker
