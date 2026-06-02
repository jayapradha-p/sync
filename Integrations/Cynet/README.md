
# Cynet

The Cynet 360 platform provides advanced threat detection, prevention and response.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root||True|String|https://<server-address>:6443/api|
|Username||True|String||
|Password||True|Password|*****|
|Verify SSL||False|Boolean|false|


#### Dependencies
| |
|-|
|requests-2.32.4-py3-none-any.whl|
|TIPCommon-1.0.11-py2.py3-none-any.whl|
|idna-3.13-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|certifi-2026.4.22-py3-none-any.whl|
|hashID-3.1.4-py2.py3-none-any.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|


## Actions
#### Hash Query
Retrieve all information about a specific file
Timeout - 600 Seconds



#### Delete Hash In Hosts
Delete file remediation action
Timeout - 600 Seconds



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Kill Hash In Hosts
Kill process file remediation action
Timeout - 600 Seconds



#### Quarantine Hash In Hosts
Quarantine file remediation action
Timeout - 600 Seconds



#### Remediation Status
Get remediation status based on remediation ID
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Remediation Id|e.g. 312|True|String||









