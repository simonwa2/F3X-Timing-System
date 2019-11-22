# piCAMTracker - Connecting to the Timing System Radio Network

The piCAMTracker unit is provided pre-configured to connect to the timing system.

There are several factors affecting connection:
### Base type
* The xbee radio module has been configured and labelled as either A or B - corresponding to Base A or Base B
* The Base Select Jumper has been set to either A or B.  It must match the xbee configuration

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/picam_left.jpg" width="376" title="piCAMTracker pi Hat">

### Antenna
* A small 2.4GHxz antenna has been provided and screws in on the top of the piCAMTracker unit.  There must be clear line of sight from the antenna to the timing system central unit or repeater.

### Connection LED
The rear LED indicates connection status:
* Solid on - indicates no connection
* Flashing on/off - indicates connected to the radio network.  It may take up to about 30 seconds to connect from when power is applied.

### Timing System
On the timing system unit being used (CD Unit, Team Unit or UniTimer), the relevant camera selection must be enabled.  The timing unit then programs the xbee radio module in piCAMTracker to send data to the CD, Team or UniTimer network address.

Note that you only need to do this process once.  Settings are retained in both the piCAMTracker xbee and in the timing system unit.

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/CD_cams.jpg" width="300" title="CD Unit">
<img align="right" src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/UniTimer_cams.jpg" width="300" title="UniTimer">
<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/Team_cams.jpg" width="300" title="Team Unit">
