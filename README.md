# hackintosh-b550mplusasustuf-rx5600xt

My (working) history versions

### hardware info
CPU: AMD Ryzen 9 3900x
GPU: Asus AMD Radeon 5600XT EVO 6GB
RAM: G.Skill Tridentz RGB 2x16GB 3600 mhz
Motherboard: Asus tuf B550M Plus Asus
Audio Codec: Realtek ALC S1200A
Ethernet Card: Realtek RTL8125B 2.5Gb
Wifi/BT Card: None
Touchpad and touch display devices: None
BIOS revision:

### Version links
Mac OS Version: Big Sur 11.1
OpenCore Version: 0.6.5

#### What works
###### Sleep / Wake
###### Ethernet 
Works, but if you're doing a clean install you need to run the following command on terminal to download the OS from Apple
`ifconfig en0 media 1000baseT`

If you already installed the OS then just go to Network -> Advanced -> Hardware -> Setup Manually -> Change speed to 1000baseT and duplex to Full-duplex
###### Imessage
###### All usb ports

#### What doesn't work
###### HDMI Monitor audio
Sometimes the hdmi monitor audio doesn't show as an option for audio output

#### Link to branch
[BigSur 11.1](/rsnchs/hackintosh-b550mplusasustuf-rx5600xt/bigsur11.1)
