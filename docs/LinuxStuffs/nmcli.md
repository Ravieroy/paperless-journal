A command-line tool for controlling NetworkManager.

```bash
Run an `nmcli` subcommand:

      nmcli agent|connection|device|general|help|monitor|networking|radio command_options

  Display the current version of NetworkManager:

      nmcli --version

  Display help:

      nmcli --help

  Display help for a subcommand:

      nmcli subcommand --help
```

## Using `nmcli` to configure static IP

- `nmcli device` : Get the listing of network interface (see sample output below).

```bash
DEVICE          TYPE      STATE         CONNECTION         
enp7s0f4u1c2    ethernet  connected     Wired connection 2 
wlp3s0          wifi      disconnected  --                 
p2p-dev-wlp3s0  wifi-p2p  disconnected  --                 
enp2s0f0        ethernet  unavailable   --                 
lo              loopback  unmanaged     --  
```

- `nmcli connection modify bssid ipv4.addresses xx.xxx.x.xxx/xx`
- `nmcli connection modify bssid ipv4.gateway xx.xxx.x.x`
- `nmcli connection modify bssid ipv4.method manual`
- `nmcli connection modify bssid ipv4.dns x.x.x.x`
- `nmcli connection down bssid && nmcli connection up bssid`
- `ip address show bssid`

## Adding secondary static IP using `nmcli`
This is for the case if we have a secondary network in environment. 

1. `nmcli device status`
2. `nmcli connection show --active`
3. `nmcli connection modify bssid +ipv4.addresses xx.x.x.xxx/xx`
4. `nmcli connection reload`
5. `systemctl reload`
6. `ip a`

