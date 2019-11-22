# piCAMTracker - Connecting to the Timing System Radio Network

The piCAMTracker unit is provided pre-configured to connect to the timing system.

There are several factors affecting connection:
### Base type
* The xbee radio module has been configured and labelled as either A or B - corresponding to Base A or Base B
* The Base Slect Jumper has been set to either A or B.  It must match the xbee configuration

### Antenna
* A small 2.4GHxz antenna has been provided and screws in on the top of the piCAMTracker unit.  There must be clear line of sight from the antenna to the timing system central unit or repeater.

### Connection LED
The rear LED indicates connection status:
* Solid on - indicates no connection
* Flashing on/off - indicates connected to the radio network.  It may take up to about 30 seconds to connect from when power is applied.


