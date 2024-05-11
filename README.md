# home-assistant-guide-and-maintenance
Home Assistant guide and maintenance.


OS Version Home Assistant OS: 12.1 (as seen in console/cli)  
Home Assistant Core: 2024.4.0

## Installation
Follow the instruction in this link https://smarthomescene.com/guides/how-to-install-home-assistant-on-proxmox-the-easy-way/

## Eufy Security
https://github.com/ejbaling/eufy_security, forked from fuatakgun/eufy_security
### Install Eufy Security Add-On https://github.com/ejbaling/hassio-eufy-security-ws, forked from bropat/hassio-eufy-security-ws
### Install Home Assistant Community Store (HACS). 
* Enable [Advanced mode] in your profile page
* Install [Terminal & SSH] from Add-on Store, use the search field to find it https://www.youtube.com/watch?v=Q8Gj0LiklRE&ab_channel=SmartHomeJunkie
* Type ```wget -O - https://get.hacs.xyz | bash -```. Restart Home Assistant.
* From Integrations Page, click ADD INTEGRATION. Search HACS and add it.
### Install go2rtc Add-on https://github.com/ejbaling/WebRTC, forked from fuatakgun/WebRTC
* From HACS page, download and install [WebRTC Camera]. Restart Home Assistant.
### Install Eufy Security Integration
* Search for ```Eufy Security``` inside ```HACS``` Integrations.
* Install ```Eufy Security```. Restart Home Assistant.
* From Integrations Page, click ADD INTEGRATION. Search ```Eufy Security`` and add it. You cannot add this if the ```Eufy Security Add-On``` is not configured and running.

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
