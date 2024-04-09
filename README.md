# home-assistant-guide-and-maintenance
Home Assistant guide and maintenance.


OS Version Home Assistant OS: 12.1 (as seen in console/cli)  
Home Assistant Core: 2024.4.0

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
