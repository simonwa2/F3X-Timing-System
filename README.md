# F3X Timing System

## About
The F3X Timing System is a wireless solution for F3F and F3B.  It has been developed and evolved over many years, primarily in response to a need to simplify event timing and management in Western Australia.  In recent years systems have been built for individuals and clubs outside of Australia.

### Simple System for Training Example
<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/SimpleSystem.jpg" width="768" title="F3F">

### Full System Example
<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/FullSystem.jpg" width="1024" title="F3F">

***
## News

### 19 January 2021
**Transition to ESP NOW radio link.**  Development of a new radio link between modules is nearing completion.  It utilises the ESP NOW protocol available on ESP8266 and ESP32 processors.  ESP NOW provides significantly lower latency and hardware cost than the Xbee modules that the timing system has used for many years.
Existing timing system units will be able to be upgraded to ESP NOW via a plug-in module that replaces the Xbee.  New units have also been developed that utilise ESP NOW.

A short video demonstrating the system is available :
https://www.youtube.com/watch?v=c-oyRrp0d6k&feature=emb_logo

The video also shows the new UniTimer V2 which is a major upgrade from the original UniTimer with an improved and larger display.

Upgrade modules and new units will available from March 2021 (subject to successful contest testing of ESP NOW in February).


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

### Uni-Timer V2
Cutdown version of CD unit.  Provides announcements for
countdowns, turn signals and flight time.  Links to base units for
completely wireless operation (and audioand wind in the near future). 
But (at the moment) does not manage contests and does not link to
f3xvault.  Only has a small screen, but provides web pages for extending
capability to smart phones.  Also much cheaper than CD Unit.  It was
originaly intended to be only used for training (particularly with
piCAMTracker), but now my intention is to extend it to full contest
management as well.

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/UniTimer V2.jpg" width="256" title="UniTimer v2">

### Repeater
Range extender for the local network that links the units.  Placed on a pole near the centre of the course.   

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/repeater_small.jpg" width="90" title="Repeater">


### Audio
Wireless audio with line out for connecting to a powered speaker.

### Display
Wireless large panel LED display for showing flight data to other pilots and watchers. High brightness colour display.  Two versions:
* 400mm x 400mm witha resolution of 64 x 64 pixels
* 260mm x 130mm with a resolution of 64 x 32 pixels

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/display_unit_1.jpg" width="256" title="Display">


## Supported Camera Systems

* Motcam
* piCAMTracker
