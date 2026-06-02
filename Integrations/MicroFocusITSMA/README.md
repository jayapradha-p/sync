
# MicroFocusITSMA

A complete automation solution to enable efficient automated service management and reduce the cost of IT operations.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|URL|https://<serverAddress>/|
|Username||True|String||
|Password||True|Password|*****|
|Tenant ID||True|String||
|External System||True|String||
|External ID||True|String||
|Verify SSL||False|Boolean||


#### Dependencies
| |
|-|
|urllib3-2.6.3-py3-none-any.whl|
|charset_normalizer-3.4.6-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|idna-3.11-py3-none-any.whl|
|requests-2.32.5-py3-none-any.whl|
|certifi-2026.2.25-py3-none-any.whl|


## Actions
#### Create Incident
Create a new incident
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Display Label|The display label of the incident|True|String|None|
|Description|The description of the incident|True|String|None|
|Impact Scope|The impact scope of the incident|True|String|None|
|Urgency|The urgency of the incident|True|String|None|
|Service ID|The id of the category of the incident|True|String|None|



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Update Incident
Update an existing incident
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Incident ID|The ID of the incident|True|String|None|
|Display Label|The updated display label of the incident|False|String|None|
|Description|The updated description of the incident|False|String|None|
|Impact Scope|The updated impact score of the incident|False|String|None|
|Urgency|The updated urgency of the incident|False|String|None|
|Service ID|The updated Id of the category of the incident|False|String|None|



#### Update Incident External Status
Update the external status for an incident
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Incident ID|The ID of the incident|True|String|None|
|Status|The updated external status of the incident|True|String|None|









