# PiCAMTracker Configuration

This section deals with setting up piCAMTracker with the pi Hat installed and connecting to one of the F3X timing system units (CD, Team or UniTimer).

The picam unit, as supplied, is configured for testing done in Western Australia and needs configuring for your local wifi and country specific settings (keyboard, language, timezone etc).

The initial configuration requies you to connect a mouse (USB), keyboard (USB) and monitor (HDMI). A TV could be used if you don't have a computer monitor.

One the unit has been connected to your home wifi, then it wil be possible to remotely connect to it using VNC Viewer on your computer.  The mouse, keyboard and monitor are then no longer required.

## Connecting the mouse, keyboard and monitor
There are four USB ports at the rear of the Raspberry Pi.  The HDMI video port is accessible from the underside of the case.

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/picam_ports.jpg" width="376" title="USB and HDMI">


## Configuring localisation settings
Power on the unit (with the mouse, keyboard and monitor connected).  The monitor will show the startup process and then a display similar to Microsoft Windows.  The mouse should be active.
* Use the mouse to select the Raspberry Pi Configuration menu:
** Preferences / Raspberry Pi Configuration
<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/picam_localisation.jpg" width="376" title="Localisation">

* Select the Localisation tab then in turn set:
** Set Locale
** Set Timezone
** Set Kyboard
** Set Wifi Country
* Click on OK and agree to a restart when prompted

Note that the camera view will partially cover the configuration window.  You can drag the window to one side to see it better.

## Passsword and Hostname
* Hostname has been preset to either "BaseA" or "BaseB".  This is what will show as the name on a web page and in VNC.
* Password has been preset to "pct".  Required when accessing the unit via VNC.

You change these to if you want from the Raspberry Pi Configuration  / System tab.

## Setting up wifi
  On the bottom right of the display is the wifi status:

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/picam_wifi.jpg" width="376" title="wifi">
  
* Click on the wifi symbol and the unit will search for available wifi routers
* Select your wifi router and enter the password

This should be done for your home wifi and also any hotspot/router that you will use at the slope - e.g. your mobile phone.

## VNC Viewer
VNC Viewer is a program that allows you to remotely access teh Raspberry Pi from a computer.  This removes the need to connect a monitor, mouse and keyboard.  For this to work the piCAMTracker unit and teh coputer must be conencted to tehsame wifi network, e.g. your home wifi.

VNC is already enabled on the Raspberry Pi.

Download VNC Viewer from here:
https://www.realvnc.com/en/connect/download/viewer/

To connect to the piCAMTracker unit:
* turn power on
* open VNC Viewer on your computer
* enter the hostname (e.g BaseA) or IP address (e.g. 192.168.0.22) of your picamTracker unit in the VNC address bar
* VNC Viewer will attempt to conenct to the unit.  You will be prompted for the login name and password.  The login name is "pi" and the password is "pct" unless you changed it.
* VNC Viewer will then show the Raspberry Pi window and you can control it from your computer.
* Note that the camera view from piCAMTracker is not shown in VNC.

<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/picam_VNC_Viewer.jpg" width="376" title="VNC">
<img src="https://github.com/simonwa2/F3X-Timing-System/blob/master/images/picam_ip_address.jpg" width="376" title="IP Address">

