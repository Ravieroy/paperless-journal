If we run the command `iwconfig` in [[Terminal]], we will see our connected devices. 
```bash
lo        no wireless extensions.

eth0      no wireless extensions.

wlan0     IEEE 802.11  ESSID:off/any  
          Mode:Managed  Access Point: Not-Associated   Tx-Power=20 dBm   
          Retry short  long limit:2   RTS thr:off   Fragment thr:off
          Power Management:off
```
The default mode of the `wlan0` is `Managed` but we need to change it to monitor mode for network hacking. 

1. Disable the interface `wlan0`
```bash
sudo ifconfig wlan0 down
```

2. Kill network-manager 
```bash
sudo airmon-ng check kill
```

The output would be something like
```bash
Killing these processes:

    PID Name
   2143 wpa_supplicant

```

3. Change the mode to `monitor`
```bash
sudo iwconfig wlan0 mode Monitor
```

4. Enable the interface
```bash
sudo ifconfig wlan0 up
```