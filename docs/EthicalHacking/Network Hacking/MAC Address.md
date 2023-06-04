- It stands for Media Access Control and is permanent, physical and unique address assigned to network device by the manufacturer. 
- It is used within the network to identify devices and transfer data between devices. 
![[mac-address.png]]

### Why change the MAC address
1. Increase anonymity 
2. Impersonate other devices 
3. Bypass filters 

### How to change MAC address 

1. Use `ifconfig` to get the details of the devices connected. It will show some common devices connected like `eth0`, `lo` and if wireless adapter is connected it will show `wlan0`. Suppose we want to change the MAC address of the wireless adapter connected. The details would be something like, (**`ether`** here is the MAC address we want to change.)
```bash
wlan0: flags=4099<UP,BROADCAST,MULTICAST>  mtu 1500
        ether 70:89:8f:23:08:y6  txqueuelen 1000  (Ethernet)
        RX packets 0  bytes 0 (0.0 B)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 0  bytes 0 (0.0 B)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0
```

2. Use the following command to disable the device before changing the MAC address. (Also see [[Some Common Errors#2. SIOCSIFFLAGS Operation not permitted and SIOCSIFHWADDR Operation not permitted|Permission Error]])
```bash
ifconfig wlan0 down
```

3. Now we use the following command to set the new address for the interface(`wlan0`)
```bash
ifconfig wlan0 hw wlan0 ether 00:11:22:33:44:55
```

4. Enable the device back up.
```bash
ifconfig wlan0 up
```

5. This MAC address won't be permanent as will revert back to original after a reboot because the above process only changes the MAC address in the memory and not the physical address. If the MAC address is getting changed even without a reboot then follow the below steps.([Youtube tutorial](https://www.youtube.com/watch?v=7AUGQNBCddo)) 

6. Use any text editor like [[Vim]] and edit the following file, `vim /etc/NetworkManager/NetworkManager.conf

7. Append the config file with the following text.
```text
[device] 
wifi.scan-rand-mac-address=no 

[connection] 
ethernet.cloned-mac-address=preserve 
wifi.cloned-mac-address=preserve
```

8. Restart the network service or restart the virtual box. 
```bash
service network-manager restart # OR 
service networking restart 
```
