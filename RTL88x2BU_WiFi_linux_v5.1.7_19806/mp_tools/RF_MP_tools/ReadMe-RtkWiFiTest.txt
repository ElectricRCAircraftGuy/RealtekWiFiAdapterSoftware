[1. Features]

The RtkWiFiTest is a sample graphic UI application which lets you do RF calibration with the Realtek WiFi driver,
Or to test RF certification. It's just for running on the Android Platform.

The Latest Formal Release
Version: 1.2.0, Date: 2016/01/04

[2. Software Package]

	a. rtwpriv source and contain of the executable file for all platforms (ARM ARM64 Intel x86 x64 MIPS MIPS64).
	b. RtkWiFiTest_Vx_. apk was an Android application GUI tool.

[3. Installation step]:

Manual installation steps:
	a. adb root
	b. adb install -r RtkWiFiTest. apk
	Or 
	c. Copy the apk to the Android system, then click it.
[4. To Manual Command for the execute MP command ]
	1. After install the apk tool, it will auto install the rtwpriv in the "/data/data/realtek.com/rtwpriv".
	2. Then copy the rtwpriv in the /system/bin/, and change file parameter #chmod 755 rtwpriv, make it had executable.
	3. To do command mode for MP operating.
	#ifconfig wlan0 up
	#rtwpriv wlan0 mp_start
	#rtwpriv wlan0 mp_channel 1
	....

[ 5. Troubleshooting ]:

1. If Fail run the manual command mode or apk can't use the rtwpriv to operating. 
	a.Please to build and compile the rtwpriv source, and run the rtwpriv tool
	b. #./rtwpriv wlan0
It should show the following Message:
	rtwpriv version:V2.0_20151130
	no enough parameters!
We must to confirm the version is V2.0_20151130.

2. If had followed Message
	Interface doesn't accept private ioctl...
	: Operation not supported on transport endpoint

a. Make sure the wlan driver be loaded, and check the wlan0 was detected.
b. Confirm whether driver has been updated to the latest version.
c. Catch the system log for Realtek FAE.


