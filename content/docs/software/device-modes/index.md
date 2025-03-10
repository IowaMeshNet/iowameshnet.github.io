---
title: Device Modes
---

Meshtastic supports various operating modes to suit different needs:

| Device Role | Description | Best Uses |
|-------------|-------------|-----------|
| CLIENT | App connected or stand alone messaging device. Rebroadcasts packets when no other node has done so. | General use for individuals needing to communicate over the Meshtastic network with support for client applications. |
| CLIENT_MUTE | Device that does not forward packets from other devices. | Situations where a device needs to participate in the network without assisting in packet routing, reducing network load. |
| CLIENT_HIDDEN | Device that only broadcasts as needed for stealth or power savings. | Use in stealth/hidden deployments or to reduce airtime/power consumption while still participating in the network. |
| TRACKER | Broadcasts GPS position packets as priority. | Tracking the location of individuals or assets, especially in scenarios where timely and efficient location updates are critical. |
| LOST_AND_FOUND | Broadcasts location as message to default channel regularly for to assist with device recovery. | Used for recovery efforts of a lost device. |
| SENSOR | Broadcasts telemetry packets as priority. | Deploying in scenarios where gathering environmental or other sensor data is crucial, with efficient power usage and frequent updates. |
| TAK | Optimized for ATAK system communication, reduces routine broadcasts. | Integration with ATAK systems (via the Meshtastic ATAK Plugin) for communication in tactical or coordinated operations. |
| TAK_TRACKER | Enables automatic TAK PLI broadcasts and reduces routine broadcasts. | Standalone PLI integration with ATAK systems for communication in tactical or coordinated operations. |
| REPEATER | Infrastructure node for extending network coverage by always rebroadcasting packets once with minimal overhead. Not visible in Nodes list. | Best positioned in strategic locations to maximize the network's overall coverage. Device is not shown in topology. |
| ROUTER | Infrastructure node for extending network coverage by always rebroadcasting packets once. Visible in Nodes list. | Best positioned in strategic locations to maximize the network's overall coverage. Device is shown in topology. |
| ROUTER_LATE | Infrastructure node that always rebroadcasts packets once but only after all other nodes, ensuring additional coverage for local clusters. Visible in Nodes list. | Ideal for covering dead spots or ensuring reliability for a cluster of nodes where placement doesn't benefit the broader mesh. Device is shown in topology. |

For more details, explore the [Meshtastic Blog](https://meshtastic.org/blog/choosing-the-right-device-role/).

Here is another great video by TheCommsChannel explaining [Different Roles](https://youtu.be/htjwtnjQkkE?si=T3gjdGik5H1nYJo4).

In the best case or you are in doubt choose client. If you have a mobile unit or traveling by plane client_mute is super helpful
