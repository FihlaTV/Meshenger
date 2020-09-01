# Uphi-Hybrid - An  hotspot Messenger 

This Android app allows voice- and video communication without any server or Internet access. Simply scan each others contact QR-Code and call each other. This works on most networks such as community networks or even company networks.


## How Does It Work?

### Finding Contacts

Contacts are found by taking the devices own IPv6 addresses and replacing the devices own MAC address by the contacts MAC address. This results in using IPv6 Link Local addresses (fe80::/10) and Unique Unicast addresses (fc00::/7 using the [EUI-64](https://de.wikipedia.org/wiki/EUI-64) format).

### Audio/Video transmission

Audio and Video are transmitted via [WebRTC](https://webrtc.org/). WebRTC is a standard that is also implemented in all major web browsers. WebRTC has facilities to circumvent NAT scenarios via servers (Meshenger does not use this feature), Audio and Video codecs and end to end encryption.

WebRTC does not support signaling and authentication. The signaling information is transmitted directly as plaintext.

## Project Context


## Ideas/Future Plans

* contact authentication via public key
* optional global connection via Internet in case no local connection is available
* optional direct connection via WiFi-Direct in case no AccessPoint is available
