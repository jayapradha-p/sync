
# SEP12

Symantec Endpoint Protection, developed by Symantec, is a security software suite, which consists of anti-malware, intrusion prevention and firewall features for servers and desktops.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root||True|None||
|Client ID||True|String||
|Client Secret||True|Password|*****|
|Refresh Token||True|String||
|Verify SSL||False|Boolean|false|


#### Dependencies
| |
|-|
|defusedxml-0.7.1-py2.py3-none-any.whl|
|certifi-2026.4.22-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|requests-2.32.4-py3-none-any.whl|
|TIPCommon-1.0.11-py2.py3-none-any.whl|
|xmljson-0.2.1-py2.py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|idna-3.13-py3-none-any.whl|


## Actions
#### GetReport
Get command status report
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Command ID|Command ID|True|String|7E975C32C71349E9BE495EC2220B902F|



##### JSON Results
```json
{"computerName": "HOST_1", "subStateId": 0, "hardwareKey": "36817A7B13C3A6317932AD9819097123", "computerId": "9C9850840A0000BD3566F8ECC8417123", "domainName": "Default", "stateId": 0, "computerIp": "1.1.1.1", "currentLoginUserName": "admin"}
```



#### ScanEndpoint
Scan an endpoint
Timeout - 600 Seconds



#### Ping
Test connectivity to Symantec Endpoint Protection 14 instance
Timeout - 600 Seconds



#### UpdateEndpoint
Updates and endpoint
Timeout - 600 Seconds



#### UpdateAndScanEndpoint
Update and scan an endpoint
Timeout - 600 Seconds









