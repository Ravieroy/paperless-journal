## Interface configuration files 
- `/etc/nsswitch.conf`
- `/etc/hosts`
- `/etc/sysconfig/network`
- `/etc/sysconfig/network-scripts/ifcfg-nic`
- `/etc/resolv.conf`

## Network Commands

1. `ping`
**Ping** is short for **Packet Internet Groper**. This command is mainly used for checking the network connectivity among host/server and host. The ping command takes the URL or IP address as input and transfers the data packet to a specified address along with a **"PING"** message. 

```bash
Ping host:

      ping host

  Ping a host only a specific number of times:

      ping -c count host

  Ping host, specifying the interval in seconds between requests (default is 1 second):

      ping -i seconds host

  Ping host without trying to lookup symbolic names for addresses:

      ping -n host

  Ping host and ring the bell when a packet is received (if your terminal supports it):

      ping -a host

  Also display a message if no response was received:

      ping -O host

```

2. `ifconfig` : Network Interface Configurator.

```bash
View network settings of an Ethernet adapter:

      ifconfig eth0

  Display details of all interfaces, including disabled interfaces:

      ifconfig -a

  Disable eth0 interface:

      ifconfig eth0 down

  Enable eth0 interface:

      ifconfig eth0 up

  Assign IP address to eth0 interface:

      ifconfig eth0 ip_address
```

3. `ifup` or `ifdown` : Tool used to enable/disable network interfaces.

```bash
Enable interface eth0:

      ifup eth0

  Enable all the interfaces defined with "auto" in `/etc/network/interfaces`:

      ifup -a
      
Disable interface eth0:

      ifdown eth0

  Disable all interfaces which are enabled:

      ifdown -a
```

4. `netstat` :  Displays network-related information such as open connections, open socket ports, etc.
```bash
List all ports:

      netstat --all

  List all listening ports:

      netstat --listening

  List listening TCP ports:

      netstat --tcp

  Display PID and program names:

      netstat --program

  List information continuously:

      netstat --continuous

  List routes and do not resolve IP addresses to hostnames:

      netstat --route --numeric

  List listening TCP and UDP ports (+ user and process if you're root):

      netstat --listening --program --numeric --tcp --udp --extend
```

5. `tcpdump` : Dump traffic on a network.

```bash
List available network interfaces:

      tcpdump -D

  Capture the traffic of a specific interface:

      tcpdump -i eth0

  Capture all TCP traffic showing contents (ASCII) in console:

      tcpdump -A tcp

  Capture the traffic from or to a host:

      tcpdump host www.example.com

  Capture the traffic from a specific interface, source, destination and destination port:

      tcpdump -i eth0 src 192.168.1.1 and dst 192.168.1.2 and dst port 80

  Capture the traffic of a network:

      tcpdump net 192.168.1.0/24

  Capture all traffic except traffic over port 22 and save to a dump file:

      tcpdump -w dumpfile.pcap port not 22

  Read from a given dump file:

      tcpdump -r dumpfile.pcap
```

