
# CBDefense

Next-generation antivirus + EDR in one cloud-delivered platform that stops commodity malware, advanced malware, non-malware attacks and ransomware

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root||True|IP_OR_HOST|https://<server-address>|
|Api Key||True|Password|*****|


#### Dependencies
| |
|-|
|pyyaml-6.0.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|python_dateutil-2.9.0.post0-py2.py3-none-any.whl|
|pygments-2.20.0-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|wcwidth-0.6.0-py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|certifi-2026.4.22-py3-none-any.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|pika-1.3.2-py3-none-any.whl|
|cbapi-1.7.10-py2.py3-none-any.whl|
|cachetools-7.0.6-py3-none-any.whl|
|packaging-26.2-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|protobuf-7.34.1-py3-none-any.whl|
|solrq-1.1.2-py2.py3-none-any.whl|
|validators-0.35.0-py3-none-any.whl|
|idna-3.13-py3-none-any.whl|
|six-1.17.0-py2.py3-none-any.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|prompt_toolkit-3.0.52-py3-none-any.whl|


## Actions
#### Get Processes
List processes by device
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Timeframe|Timeframe of the search. e.g. 3h|True|String||



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Change Policy
Change device policy
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Policy Name|The new policy name. e.g. TEST_Policy|True|String||



#### Delete Policy
Delete a policy from Cb Defense
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Policy Name|Policy name|True|String|None|



#### Create Policy
Create a new Policy on Cb Defense
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Policy Name|Name for the policy|True|String|None|
|Policy Description|A description of the policy|True|String|None|
|Priority Level|The priority score associated with sensors assigned to this policy. e.g. LOW|True|String||
|Policy Details|The policy details|True|String|None|



#### Get Events
Get events by entity
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Timeframe|Timeframe of the search. e.g. 3h|True|String||



#### Get Device Info
Get information about a device
Timeout - 600 Seconds



#### Delete Rule From Policy
Remove a rule from an existing policy
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Policy Name|Policy name|True|String|None|
|Rule ID|Rule ID. e.g. 1|True|String|None|









