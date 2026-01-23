A Meshtastic device (SBC or microcontroller with a LoRa radio) listens on a single channel slot. That slot is derived from hashing your channel name (or from how you hard-code the config). Most people around here are using the default LongFast channel with the default key, which ends up on channel slot 20. That’s why the local mesh tends to “just work” for RF.

When packets come in over LoRa, the Meshtastic firmware tries to decrypt them using your configured channel keys. If decryption succeeds, the message is displayed to you (screen, phone, etc). If the packet matches the Meshtastic protocol but cannot be decrypted, it is still rebroadcast so other radios that might have the correct key can receive it. In this way, your node participates in the mesh automatically at the RF level.

Meshtastic can also be configured to use MQTT to relay packets over IP (usually the internet). Each packet contains flags indicating whether it is allowed to be relayed to MQTT and whether it originated from MQTT. In your settings, you can enable Ignore MQTT, which causes your device to drop MQTT-originated packets entirely.

If you enable MQTT on your device, each channel has two relevant settings:

Uplink – send RF packets to MQTT

Downlink – send MQTT packets back out over RF

These control how your node bridges between RF and MQTT.

For a LoRa-only client to receive messages that originated elsewhere via MQTT, you must not have Ignore MQTT enabled (this is the default). If you see MQTT nodes in your node list, you are probably already accepting MQTT traffic.

However, the node that is doing the MQTT bridging must:

Have the same channel configured, and

Be both uplinking and downlinking on that channel.

If a relay node is uplinking only, you’ll show up on maps and node lists, but messages won’t make it back to you. If it’s downlinking only, it won’t forward local RF traffic to MQTT.

I’ve seen a lot of mixed configurations: uplink only, downlink only, only on LongFast but not on IROMesh, etc. Depending on how those relays are set up, communication may or may not actually work end-to-end.

So:

If you see yourself on the map → someone near you is uplinking your channel.

If you see nodes but not messages → the relay probably isn’t downlinking that channel.

The only real fix is to coordinate with whoever runs the relay nodes, or run your own MQTT bridge.

One opinion on how it "should be configured":  It’s fine to uplink LongFast, but probably not wise to downlink LongFast due to volume. For a custom channel like IROMesh to work over MQTT, the relay nodes must have that channel configured and be both uplinking and downlinking it.

Also, everyone who wants to participate via MQTT needs to have “OK to MQTT” enabled on that channel.