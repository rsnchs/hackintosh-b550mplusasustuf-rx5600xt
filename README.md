# hackintosh-b550mplusasustuf-rx5600xt

My (working) history versions

### hardware info
CPU: AMD Ryzen 9 3900x

GPU: Asus AMD Radeon 5600XT EVO 6GB

RAM: G.Skill Tridentz RGB 2x16GB 3600 mhz

Motherboard: Asus tuf B550M Plus

Audio Codec: Realtek ALC S1200A

Ethernet Card: Realtek RTL8125B 2.5Gb

Wifi/BT Card: None

Touchpad and touch display devices: None

BIOS revision:

# Version History

## Mac OS Version: Big Sur 11.1

OpenCore Version: 0.6.5

#### What works

**Multi monitor**

**Sleep / Wake**

**Ethernet** 
Works, but if you're doing a clean install you need to run the following command on terminal to download the OS from Apple
`ifconfig en0 media 1000baseT`

If you already installed the OS then just go to Network -> Advanced -> Hardware -> Setup Manually -> Change speed to 1000baseT and duplex to Full-duplex

**Imessage**
**All usb ports**

Probably everything not listed

#### What doesn't work
**HDMI Monitor audio**

Sometimes the hdmi monitor audio doesn't show as an option for audio output

**Weird video glitch right before the mac OS gui loads**

This only happened after I added [this SSDT to improve the gpu performance](https://www.tonymacx86.com/threads/amd-radeon-performance-enhanced-ssdt.296555/), but only happens for a second


**AMD SVM**
So if you're developing for android you might have to use your physical device (with vysor) or use genymotion, the regular android emulatores won't work

#### Link to branch
[BigSur](https://github.com/rsnchs/hackintosh-b550mplusasustuf-rx5600xt/tree/bigsur11.1)


## Mac OS Version: Catalina 10.15.7

OpenCore Version: 0.6.2

#### What works

** Multi monitor **

**Ethernet** 
Works, but if you're doing a clean install you need to run the following command on terminal to download the OS from Apple
`ifconfig en0 media 1000baseT`

If you already installed the OS then just go to Network -> Advanced -> Hardware -> Setup Manually -> Change speed to 1000baseT and duplex to Full-duplex

**Imessage**

**All usb ports**

Probably everything not listed

#### What doesn't work

**Sleep / Wake / Restart / Turn off**

You have to unplug after shut down or it won't start, you get a black screen after POST

**AMD SVM**

So if you're developing for android you might have to use your physical device (with vysor) or use genymotion, the regular android emulatores won't work

**Video card performance**

It's not as good, you might consider adding [this SSDT to improve the gpu performance](https://www.tonymacx86.com/threads/amd-radeon-performance-enhanced-ssdt.296555/)

#### Link to branch
[Catalina](https://github.com/rsnchs/hackintosh-b550mplusasustuf-rx5600xt/tree/catalina10.15.7)
