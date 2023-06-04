1. Gathering information by [[Packet Sniffing]] about the local wireless networks. This includes 
	1. getting the `BSSID` of the network,  
	2. channel `CH` it is working on, 
	3. type of encryption(WEP/WPA/WPA2)
	4. frequency it is working on (2.4GHz/5GHz)
	5. and some more.
2. Starting a [[Targeted Packet Sniffing]] and using _wireshark_ to get more information about the devices connected to the network. From this we can get
	1. the type of device connected to the network.
	2. `ESSID` of the device. 
	3. more depending on the information _wireshark_ can provide.
3. A [[Deauthentication Attack]] can be launched on a particular device connected to the network. This can be helpful in social engineering the target users. 