
# McAfeeNSM

McAfee Network Security Platform is a next-generation intrusion prevention system (IPS) that redefines how organizations block advanced threats.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|URL|https://x.x.x.x/sdkapi/|
|Username||True|String||
|Password||True|Password|*****|
|Domain ID||True|String||
|Siemplify Policy Name||True|String||
|Sensors Names List Comma Separated||True|String|sensor_name1,sensor_name2,sensor_name3|


#### Dependencies
| |
|-|
|certifi-2026.2.25-py3-none-any.whl|
|charset_normalizer-3.4.6-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|requests-2.32.5-py3-none-any.whl|
|idna-3.11-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|


## Actions
#### Is IP Blocked
Check if an IP address is blocked
Timeout - 600 Seconds



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Quarantine IP
Quarantine a particular IP address
Timeout - 600 Seconds



#### Unblock IP
Unblock a particular IP address
Timeout - 600 Seconds



#### Get Alert Info Data
Get alert data by id.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Alert ID|Alert ID|True|String|None|
|Sensor Name|Sensor Name|True|String|None|



#### Block IP
Block IP address
Timeout - 600 Seconds









