
# Runners

Run commands as different users. Permission to replace a process level token is required (in local policies)

Python Version - 3


#### Dependencies
| |
|-|
|pytest-9.0.3-py3-none-any.whl|
|pygments-2.20.0-py3-none-any.whl|
|iniconfig-2.3.0-py3-none-any.whl|
|pluggy-1.6.0-py3-none-any.whl|
|packaging-26.2-py3-none-any.whl|
|pytest_mock-3.15.1-py3-none-any.whl|


## Actions
#### Run Command As User
Run a command as a user (Windows only)
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Command|The command to run, e.g: whoami|True|String||
|Username|Username|True|String||
|Domain|User's domain.|True|String||
|Password|Password|True|Password|*****|
|Daemon|Whether to run in the background or not|False|Boolean|true|



#### Ping
Test Connectivity
Timeout - 600 Seconds









