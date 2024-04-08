# home-assistant-guide-and-maintenance
Home Assistant guide and maintenance.


OS Version Home Assistant OS: 12.1 (as seen in console/cli)  
Home Assistant Core: 2024.4.0

## Disable newly added entities and polling for updates.
The following integrations can break if these 2 options are enabled.
* Eufy Security
* HACS
* Home Assistant Supervisor
* Mobile App
* SmartThings
* Tailscale
* WebRTC Camera

