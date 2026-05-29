
# McAfeeWebGateway

High-performance web security delivered on premises

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Server Address|None|True|String|{ip}:{port}|
|Username|None|True|String||
|Password|None|True|Password|*****|


#### Dependencies
| |
|-|
|defusedxml-0.7.1-py2.py3-none-any.whl|


## Actions
#### Block IP
Insert IP addresses to an "IP range"-type group (Note - This group should be a part of rule used to block IP addresses)
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Group Name|The group name|True|String||
|Description|The entry description|False|String|None|



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Remove Item From Group
Remove a network object to a group (ip, url, etc.). \n*Please note - that each group is type stricted
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Group Name|The group name|True|String||
|Item To Delete|The item to delete from the group. Default: x.x.x.x/32|True|String||



#### Unblock IP
Delete IP addresses from an "IP range"-type group. \n*Please note - This group should be a part of rule used to block IP addresses
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Group Name|The group name to unblock the IP in|True|String||



#### Insert Item To Group
Insert a network object to a group (ip, url, etc.). \n*Please note - that each group is type stricted
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Group Name|The group name|True|String||
|Item To Insert|The item ot insert to the group. Default: x.x.x.x/24|True|String||
|Description|The entry description|False|String||









