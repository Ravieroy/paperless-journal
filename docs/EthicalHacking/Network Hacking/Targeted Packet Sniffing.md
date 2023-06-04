Once we get the details of our target from [[Packet Sniffing]], we can then start an start our focused attack on that target. For this we will need `BSSID` and `CH` details of the network. 

```bash
sudo airodump-ng --bssid BSSID --channel CH --write output wlan0
```

This will create several files which will contain important details captured during the sniffing process. This file though is highly encrypted. We can see the details using another GUI program
called [[Wireshark]]

```bash
wireshark
```

This will open up a GUI window where we can select our `output-01.cap` file to see some details.

