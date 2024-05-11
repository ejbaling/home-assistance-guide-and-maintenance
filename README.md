# home-assistant-guide-and-maintenance
Home Assistant guide and maintenance.


OS Version Home Assistant OS: 12.1 (as seen in console/cli)  
Home Assistant Core: 2024.4.0

## Installation
Follow the instruction in this link https://smarthomescene.com/guides/how-to-install-home-assistant-on-proxmox-the-easy-way/

## Eufy Security
https://github.com/ejbaling/eufy_security, forked from fuatakgun/eufy_security

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
