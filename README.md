# home-assistant-guide-and-maintenance
Home Assistant guide and maintenance.


OS Version Home Assistant OS: 12.1 (as seen in console/cli)  
Home Assistant Core: 2024.4.0

## Installation
Follow the instruction in this link https://smarthomescene.com/guides/how-to-install-home-assistant-on-proxmox-the-easy-way/

## Eufy Security
https://github.com/ejbaling/eufy_security, forked from fuatakgun/eufy_security
Summary:
### Install Eufy Security Add-On https://github.com/ejbaling/hassio-eufy-security-ws, forked from bropat/hassio-eufy-security-ws
2. Install Home Assistant Community Store (HACS). You must nable [Advanced mode] in your profile page to install this.
3. Install go2rtc Add-on https://github.com/ejbaling/WebRTC, forked from fuatakgun/WebRTC

## Disable newly added entities and polling for updates.
Other integrations can break if these 2 options are enabled on the following integrations.
* HACS
* Home Assistant Supervisor
* WebRTC Camera

## Disable Home Assisstant Supervisor auto update.
Execute from console
```
supervisor options --auto-update=false
```
