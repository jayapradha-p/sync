
# SEP

Symantec Endpoint Protection, developed by Symantec, is a security software suite, which consists of anti-malware, intrusion prevention and firewall features for servers and desktops.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Username|None|True|String|None|
|Password|None|True|Password|*****|
|Domain|None|True|String|None|
|Api Root|None|True|URL|https://{IP}:{PORT}/sepm|
|Verify SSL|None|False|Boolean|False|


#### Dependencies
| |
|-|
|defusedxml-0.7.1-py2.py3-none-any.whl|
|chardet-5.2.0-py3-none-any.whl|
|requests-2.31.0-py3-none-any.whl|
|certifi-2024.2.2-py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|idna-3.7-py3-none-any.whl|
|urllib3-2.2.1-py3-none-any.whl|
|xmljson-0.2.1-py2.py3-none-any.whl|
|TIPCommon-1.0.12-py2.py3-none-any.whl|


## Actions
#### DisableNTP
Disable NTP on endpoints
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Time Period|Time Period|True|String|5|



#### GetSystemInfo
Get system information for endpoints
Timeout - 600 Seconds



#### Get Report And Enrich
Get command status report and enrich entities
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Command IDS|Command IDS|True|String|7E975C32C71349E9BE495EC2220B902F|



#### EnableDownloadInsight
Enable Download Insight on endpoints
Timeout - 600 Seconds



#### GetReport
Get command status report
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Command IDS|Command IDS|True|String|7E975C32C71349E9BE495EC2220B902F|



#### ListEndpoints
 List all the endpoints/sensors configured on a particular device
Timeout - 600 Seconds



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### QuarantineEndpoint
Quarantine an endpoint
Timeout - 600 Seconds



#### UnblockHash
Unblock a particular hash
Timeout - 600 Seconds



#### UpdateEndpoint
Update an endpoint
Timeout - 600 Seconds



#### BlockHash
Blocks a particular hash on endpoints
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Black List Name|The black list name to add the hash to|True|String||



#### UnquarantineEndpoint
Unquarantine an endpoint
Timeout - 600 Seconds



#### UpdateAndScanEndpoint
Update and scan an endpoint
Timeout - 600 Seconds



#### DisableDownloadInsight
Disable Download Insight on endpoints
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Time Period|Time Period|True|String|5|



#### EnableNTP
Enable NTP on endpoints
Timeout - 600 Seconds



#### ScanEndpoint
Scan an endpoint
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Scan Type|The type of the scan to perform. ScanNow_Full = Full scan, ScanNow_Quick = quick scan, ScanNow_Custom = custom scan.|True|List|ScanNow_Full|



#### ListGroups
List all the groups configured on a particular device
Timeout - 600 Seconds









