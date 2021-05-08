[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FElectricRCAircraftGuy%2FRealtekWiFiAdapterSoftware&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=views+%28today+%2F+total%29&edge_flat=false)](https://hits.seeyoufarm.com)

# Repo Status

Ready to use. Here are the files. 


# Table of Contents
<details>
<summary><b>(click to expand or hide)</b></summary>
<!-- MarkdownTOC -->

1. [All of my Wifi adapter repos:](#all-of-my-wifi-adapter-repos)
1. [RealtekWiFiAdapterSoftware](#realtekwifiadaptersoftware)
    1. [Testing:](#testing)
    1. [Installation Instructions:](#installation-instructions)

<!-- /MarkdownTOC -->
</details>


<a id="all-of-my-wifi-adapter-repos"></a>
# All of my Wifi adapter repos:

- **If you are using Linux and desire a high-speed WiFi adapter, I recommend [this BrosTrend Wifi adapter](https://amzn.to/33qXt9i) above all others! It installs with a simple 1-line or 3-line command and has an excellent installation script, as well as great performance, speed, and range.** 
- If you are using Linux and need a Wifi adapter which is _plug-and-play_ and requires NO driver installation, _and_ are okay with it being a bit slower than the BrosTrend one above, then buy a [Panda Wifi adapter like this one](https://amzn.to/2Q0JnZd) instead.

My Wifi Repositories:
1. [BrosTrendWifiAdapterSoftware](https://github.com/ElectricRCAircraftGuy/BrosTrendWifiAdapterSoftware) - (BEST WIFI ADAPTER FOR LINUX, HANDS-DOWN!)
1. [AlfaWiFiAdapterSoftware](https://github.com/ElectricRCAircraftGuy/AlfaWiFiAdapterSoftware)
1. [RealtekWiFiAdapterSoftware](https://github.com/ElectricRCAircraftGuy/RealtekWiFiAdapterSoftware)


<a id="realtekwifiadaptersoftware"></a>
# RealtekWiFiAdapterSoftware
Software that comes on a tiny little CD with the ["LGTERK 1200Mbps USB 3.0 Wifi Adapter" from Amazon](http://amzn.to/2ECm4ul). The words printed on the CD label say the following:
```
802.11AC 
Drivers&Utilities

Win XP,Vista,Win7,Win8,Win10
MacOS_Driver
WIFI_Linux_Driver
Ver:BU1109
```

Since not all computers even have CD drives today, it's nice to have a way to download the drivers instead. So, here they are. 

Chipset: Realtek 8812BU Wireless LAN 802.11ac USB NIC

<a id="testing"></a>
## Testing:

 * Windows: works great once you manually install the driver from the CD! Without manually installing the driver it doesn't work at all. 
   * AP (Access Point) mode also works really well for turning this device into a WiFi hot spot! Ex scenario: Use your laptop to connect to the internet via some other way (ex: internal WiFi adapter, Ethernet cable, or tethered phone), then put this external WiFi adapter into AP mode!
   * To put into AP mode: right-click the new "REALTEK USB Wireless LAN Utility" icon (a row of increasing-height green vertical bars) in the System Tray and go to "Open Config Utility", then in the GUI that opens up, click "Mode" --> "Access Point." 
     * WARNING: Use other GUI settings here to set a password or else your access point will be open to the public. 
 * Linux:
   * Ubuntu 14.04 LTS:
     * Tested and works well! See Linux install instructions below.
     * Speeds (using [`speedtest-cli`](https://www.howtoforge.com/tutorial/check-internet-speed-with-speedtest-cli-on-ubuntu/) tool) on my high-end laptop in a USB 3.0 port were 100~200 Mbps download and upload, which is about 1/2 as fast as the built-in WiFi card on my 1Gbps internet connection.
     * AP mode not tested
 * Mac OS: unk

<a id="installation-instructions"></a>
## Installation Instructions:

 * Windows: double-click the `Windows_driver/Setup.exe` file. 
 * Linux Ubuntu: 
   * In folder manager, right-click `RealtekWiFiAdapterSoftware-master.zip` and go to "Extract Here"
   * Once extracted, open up a terminal and `cd` into `RealtekWiFiAdapterSoftware-master/RTL88x2BU_WiFi_linux_v5.1.7_19806`
   * ENSURE THAT NO SPACES EXIST ANYWHERE IN THE ENTIRE PATH NAME, OR ELSE THE FOLLOWING STEPS MAY FAIL. LINUX IS NOTORIOUS FOR REQUIRING THAT COMMAND-LINE COMPILATION AND INSTALLATION TOOLS RUN ONLY IN DIRECTORIES NOT CONTAINING SPACES. Once in the directory which contains the `install.sh` file, run the following commands: 
   * `chmod +x install.sh`
   * `sudo ./install.sh`
   * Done! Click the WiFi symbol at the top of the screen in Ubuntu and select the hotspot you'd like to connect to with the new "Realtek USB3.0 802.11ac 1200M Adapter" now showing up in the menu.

Cheers! For more useful computer, electronics, Arduino, Linux, Radio Control and other articles and tips, visit me at www.ElectricRCAircraftGuy.com.

Disclaimer.  
*Even though I bought this device with my own money, unsolicited, and am not being paid to write anything about this product, I am required to post the following disclaimer: "We are a participant in the Amazon Services LLC Associates Program, an affiliate advertising program designed to provide a means for us to earn fees by linking to Amazon.com and affiliated sites."*
