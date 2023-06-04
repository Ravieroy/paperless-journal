`systemctl` command is a tool to control system services. It replaces the older command `service`

### Usage Syntax

```bash
systemctl start|stop|status servicename.service
systemctl enable servicename.service
systemctl restart|reload servicename.service
systemctl list-units --all
```

```bash
- Show all running services:
    systemctl status

  - List failed units:
    systemctl --failed

  - Start/Stop/Restart/Reload a service:
    systemctl start|stop|restart|reload unit

  - Show the status of a unit:
    systemctl status unit

  - Enable/Disable a unit to be started on bootup:
    systemctl enable|disable unit

  - Mask/Unmask a unit to prevent enablement and manual activation:
    systemctl mask|unmask unit

  - Reload systemd, scanning for new or changed units:
    systemctl daemon-reload

  - Check if a unit is enabled:
    systemctl is-enabled unit
```

The output has following columns : 

- **UNIT :**  The `systemd` unit name

- **LOAD :** Whether the unit's configuration has been parsed by `systemd`. The configuration of loaded units is kept in memory.

- **ACTIVE :** A summary state about the unit is active.

- **SUB :** This is a lower-level state that indicates more detailed information about the unit. 

- **DESCRIPTION :** A short textual description of what the unit is/does

### Usage Examples

1. To see status of Bluetooth
```bash
systemctl status bluetooth
```

**Output**
```bash
bluetooth.service - Bluetooth service
     Loaded: loaded (/usr/lib/systemd/system/bluetooth.service; enabled; preset: enabled)
     Active: active (running) since Sat 2023-05-27 15:09:13 IST; 20h ago
       Docs: man:bluetoothd(8)
   Main PID: 1067 (bluetoothd)
     Status: "Running"
      Tasks: 1 (limit: 18163)
     Memory: 2.7M
        CPU: 153ms
     CGroup: /system.slice/bluetooth.service
             └─1067 /usr/libexec/bluetooth/bluetoothd
```

2. To stop the Bluetooth
```bash
systemctl stop bluetooth
```

3. To disable at boot
```bash
systemctl disable bluetooth
```


### Add a service under `systemctl` management

Inorder to add a service, create a unit file in `/etc/systemd/system/servicename.service`
where `servicename.service` is the name of service to be added. 

### To control system with `systemctl`

1. `systemctl poweroff`
2. `systemctl halt`
3. `systemctl reboot`
