## MobileAnchor
Mobile anchor is a small project that turns a base Raspbian installation to a WiFi hotspot and DHCP server.
It also features basic file serving abilities through minidlna and a samba server

## Features
- Creates a WiFi Network to connect phones, tablets and computers together
- Automatically mounts USB storage devices to `/mnt` directory
- Serves `/mnt` directory content through DLNA and CIFS

## Use case
I use Mobile Anchor primarily to build a media server for the car, but the possibilities are endless once you
get devices to connect together like tablets, phones and computers on the same WiFi network.

[VLC](http://www.videolan.org/) on [iOS](http://www.videolan.org/vlc/download-ios.html), or [Android](http://www.videolan.org/vlc/download-android.html) can access and playback media content.

## Installing
Edit the `config` file to setup your WiFi access point and key, then run the `install` script with sudo.
```
$ cp config.sample config
$ cat config
# WiFi Network Name
SSID MySSID

# Wifi Key
WIFI_KEY Sup3rS3cretKey

# IP Address
IP_ADDRESS 192.168.101.1
NETMASK 255.255.255.0

# DHCP start/end
DHCP_START 192.168.101.100
DHCP_END 192.168.101.200
$ sudo ./install
```
