
# SSH

Connect to endpoints vis SSH and perform various operations.

Python Version - 3


#### Dependencies
| |
|-|
|bcrypt-5.0.0-cp39-abi3-manylinux2014_x86_64.manylinux_2_17_x86_64.whl|
|paramiko-3.4.0-py3-none-any.whl|
|pynacl-1.6.2-cp38-abi3-manylinux2014_x86_64.manylinux_2_17_x86_64.whl|
|iniconfig-2.3.0-py3-none-any.whl|
|packaging-26.2-py3-none-any.whl|
|pycparser-3.0-py3-none-any.whl|
|pytest_mock-3.15.1-py3-none-any.whl|
|pytest-9.0.3-py3-none-any.whl|
|cryptography-46.0.7-cp311-abi3-manylinux2014_x86_64.manylinux_2_17_x86_64.whl|
|pluggy-1.6.0-py3-none-any.whl|
|cffi-2.0.0-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.whl|
|pygments-2.20.0-py3-none-any.whl|


## Actions
#### List iptables Rules
List iptables rules on a remote machine
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Remote Server|Remote server address(e.g: x.x.x.x)|True|String||
|Remote Username|Remote Username|True|String||
|Remote Password|Remote Password|True|Password|*****|
|Remote Port|The default port will be 22.|False|String||
|Chain|The iptables chain that you wish to see (e.g: INPUT, OUTPUT, etc.)|False|String||



##### JSON Results
```json
{"-,Chain,Rule": ["-P,INPUT,ACCEPT", "-P,FORWARD,ACCEPT", "-P,OUTPUT,ACCEPT"]}
```



#### List Connections
List all  connections on a remote machine
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Remote Server|Remote server address(e.g: x.x.x.x).|True|String||
|Remote Username|Remote Username|True|String||
|Remote Password|Remote Password|True|Password|*****|
|Remote Port|Remote Port|False|String||



##### JSON Results
```json
{"Results": ["Proto,Recv-Q,Send-Q,Local,Address,Foreign,Address,State,PID/Program,name", "tcp,0,0,0.0.0.0:111,0.0.0.0:*,LISTEN,1/systemd", "tcp,0,0,0.0.0.0:22,0.0.0.0:*,LISTEN,10624/sshd"]}
```



#### Block IP Address in iptables
Add rule to iptables to block IP address
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Remote Server|Remote server address(e.g: x.x.x.x).|True|String|x.x.x.x|
|Remote Username|Remote Username|True|String|root|
|Remote Password|Remote Password|True|Password|*****|
|Remote Port|Remote Port|False|String||
|Block IP Address|IP address to block(e.g: x.x.x.x).|True|String||



#### Run Command
Run command on a remote machine
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Remote Server|Remote server address(e.g: x.x.x.x).|True|String||
|Remote Username|Remote Username|True|String||
|Remote Password|Remote Password|True|Password|*****|
|Remote Port|Remote Port|False|String||
|Command|Command content(e.g: ifconfig).|True|String||



##### JSON Results
```json
{"ifconfig": "ens32: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>mtu1500\ninet1.1.1.1netmask1.1.1.1broadcast1.1.1.1\ninet6fe80: : 2156: 9c37: 7a0d: 87eprefixlen64scopeid0x20<link>\nether00: 50: 56: b5: 70: e3txqueuelen1000(Ethernet)\nRXpackets7448423bytes1077754116(1.0GiB)\nRXerrors0dropped0overruns0frame0\nTXpackets370155bytes44300304(42.2MiB)\nTXerrors0dropped0overruns0carrier0collisions0\n\nlo: flags=73<UP,LOOPBACK,RUNNING>mtu65536\ninet1.1.1.1netmask1.1.1.1\ninet6: : 1prefixlen128scopeid0x10<host>\nlooptxqueuelen1000(LocalLoopback)\nRXpackets86bytes4780(4.6KiB)\nRXerrors0dropped0overruns0frame0\nTXpackets86bytes4780(4.6KiB)\nTXerrors0dropped0overruns0carrier0collisions0\n\n", "output": "ens32: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>mtu1500\ninet1.1.1.1netmask1.1.1.1broadcast1.1.1.1\ninet6fe80: : 2156: 9c37: 7a0d: 87eprefixlen64scopeid0x20<link>\nether00: 50: 56: b5: 70: e3txqueuelen1000(Ethernet)\nRXpackets7448423bytes1077754116(1.0GiB)\nRXerrors0dropped0overruns0frame0\nTXpackets370155bytes44300304(42.2MiB)\nTXerrors0dropped0overruns0carrier0collisions0\n\nlo: flags=73<UP,LOOPBACK,RUNNING>mtu65536\ninet1.1.1.1netmask1.1.1.1\ninet6: : 1prefixlen128scopeid0x10<host>\nlooptxqueuelen1000(LocalLoopback)\nRXpackets86bytes4780(4.6KiB)\nRXerrors0dropped0overruns0frame0\nTXpackets86bytes4780(4.6KiB)\nTXerrors0dropped0overruns0carrier0collisions0\n\n"}
```



#### Terminate Process
Terminate process on a remote machine
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Remote Server|Remote server address(e.g: x.x.x.x)|True|String||
|Remote Username|Remote Username|True|String||
|Remote Password|Remote Password|True|Password|*****|
|Remote Port|Remote Port|False|String||
|PROCESS|Process to terminate.|True|String||



#### Delete Firewall Rule
Delete iptables Firewall rule (Example: INPUT -s 10.0.0.10 -j DROP)
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Remote Server|Remote server address(e.g: x.x.x.x).|True|String||
|Remote Username|Remote Username|True|String|root|
|Remote Password|Remote Password|True|Password|*****|
|Remote Port|Remote Port|False|String|None|
|IPtables Rule|Rule value(e.g: INPUT -s 10.0.0.10 -j DROP)|True|String||



#### Execute Program
Run script on a remote machine
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Remote Server|Remote server address(e.g: x.x.x.x).|True|String||
|Remote Username|Remote Username|True|String||
|Remote Password|Remote Password|True|Password|*****|
|Remote Port|Remote Port|False|String||
|Remote Program Path|The path to the program in the remote host.|True|String||



#### Logoff User
Log off remote user
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Remote Server|Remote server address(e.g: x.x.x.x)|True|String||
|Remote Username|Remote Username|True|String||
|Remote Password|Remote Password|True|Password|*****|
|Remote Port|The default port will be 22.|False|String||
|Logoff Username|The username to log off.|True|String||



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### List Processes
List running processes on a remote machine
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Remote Server|Remote server address(e.g: x.x.x.x).|True|String||
|Remote Username|Remote Username|True|String||
|Remote Password|Remote Password|True|Password|*****|
|Remote Port|The default port will be 22.|False|String|22|



##### JSON Results
```json
{"Processes": ["USER,PID,%CPU,%MEM,VSZ,RSS,TTY,STAT,START,TIME,COMMAND", "root,1,0.0,0.0,193656,6656,?,Ss,Jan16,0:24,/usr/lib/systemd/systemd --system --deserialize 24", "root,32142,0.0,0.0,0,0,?,S,Jan22,0:32,[kworker/3:1]"]}
```



#### Shutdown Machine
Shutdown remote machine
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Remote Server|Remote server address(e.g: x.x.x.x)|True|String||
|Remote Username|Remote Username|True|String||
|Remote Password|Remote Password|True|Password|*****|
|Remote Port|The default port will be 22.|False|String||
|Wait Time|Time to wait before shutdown in minutes(e.g: now).|True|String||



#### Reboot Machine
 Reboot remote server
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Remote Server|Remote server address(e.g: x.x.x.x).|True|String||
|Remote Username|Remote Username|True|String||
|Remote Password|Remote Password|True|Password|*****|
|Remote Port|The default port will be 22.|False|String||









