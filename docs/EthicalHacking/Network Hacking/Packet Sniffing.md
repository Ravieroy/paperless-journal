## Using `airodump-ng`
- It is a part of the `aircrack-ng` suit.
- `airodump-ng` is a packet sniffer.
- used to capture all packets within range.
- display detailed info about networks around us like connected clients.

1. [[MAC Address#How to change MAC address|Change MAC address]] (optional)

2. [[Wireless Modes|Put the wireless adapter in `Monitor` mode]]

4. Start the packet sniffer 
```bash
sudo airodump-ng wlan0
```

If your wireless adapters support 5GHz band then, the following command can be used to sniff devices working in 5GHz range.

```bash
sudo airodump-ng --band a wlan0
```

It will start scanning the network around us and the out will be somewhat like, 
```bash
CH 13 ][ Elapsed: 12 s ][ 2023-05-27 06:07

BSSID              PWR  Beacons    #Data, #/s  CH   MB   ENC CIPHER  AUTH ESSID

20:37:06:A5:8E:82  -53        4        0    0  11  130   WPA2 CCMP   MGT  STUDENT_SECURED
20:37:06:A5:8E:83  -52        6        0    0  11  130   WPA2 CCMP   MGT  GUEST_SECURED
20:37:06:A5:8E:84  -52        6        1    0  11  130   WPA2 CCMP   MGT  CAMPUS_SECURED
62:01:94:42:09:77  -60        4        1    0   1   48   WPA2 CCMP   PSK  DALIVEPP

BSSID              STATION            PWR   Rate    Lost    Frames  Notes  Probes
(not associated)   60:01:94:42:09:77  -58    0 - 1     37        7         CAMPUS
```

`BSSID` : MAC address of the wireless device. 
`PWR` : The strength of the wireless.
`Beacons` : Broadcasting the info to other devices. 
`#DATA` : Number of data packets.
`#/s` : Number of data packets per second.
`CH` :  Channel on which the network is working on.
`ENC` :  Encryption(WEP/WPA/WPA2)
`CIPHER` : Cipher used in the network
`AUTH` : Authentication used in the network.
`ESSID` : name of the network.

Also Read : 
1. [[Targeted Packet Sniffing]]
2. [[Deauthentication Attack]]


