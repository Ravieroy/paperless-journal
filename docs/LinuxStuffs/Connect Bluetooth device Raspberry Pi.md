## Terminal 
```bash
sudo bluetoothctl

agent on

default-agent

scan on

trust <device ID>
trust 50:E6:66:2E:59:EB

connect <device ID>
```

This should connect the device successfully. We can check the device using `paired-devices` command.

[LINK](http://wiki.sunfounder.cc/index.php?title=Connecting_Raspberry_Pi_with_the_Bluetooth_keyboard)
