## MobileAnchor
Mobile anchor is a small project that turns a base Raspbian installation to a WiFi hotspot and DHCP server.
It also features basic file serving abilities through minidlna and a samba server

## Use case
I use Mobile Anchor primarily to build a media server for the car, but the possibilities are endless once you
get a device that connects together tablets, phones and computers on the same WiFi network

## Installing
Edit the `config` file to setup your WiFi access point and key, then run the `install` script with sudo.
```
$ cat config 
SSID MySSID
WIFI_KEY Sup3rS3cretKey
$ sudo ./install
```
