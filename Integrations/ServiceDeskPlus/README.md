
# ServiceDeskPlus

ServiceDesk Plus is a game changer in turning IT teams from daily fire-fighting to delivering awesome customer service.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root|None|True|String|http://{IP or FQDN}/sdpapi/|
|Api Key|None|True|Password|*****|


#### Dependencies
| |
|-|
|defusedxml-0.7.1-py2.py3-none-any.whl|
|idna-3.15-py3-none-any.whl|
|certifi-2026.4.22-py3-none-any.whl|
|google_api_python_client-2.188.0-py3-none-any.whl|
|pyopenssl-25.3.0-py3-none-any.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|pycparser-3.0-py3-none-any.whl|
|httpx-0.28.1-py3-none-any.whl|
|google_auth_httplib2-0.3.0-py3-none-any.whl|
|httpcore-1.0.9-py3-none-any.whl|
|uritemplate-4.2.0-py3-none-any.whl|
|rsa-4.9.1-py3-none-any.whl|
|pyparsing-3.3.2-py3-none-any.whl|
|xmltodict-0.13.0-py2.py3-none-any.whl|
|h11-0.16.0-py3-none-any.whl|
|anyio-4.13.0-py3-none-any.whl|
|requests-2.32.5-py3-none-any.whl|
|google_auth-2.47.0-py3-none-any.whl|
|urllib3-2.7.0-py3-none-any.whl|
|protobuf-7.34.1-cp310-abi3-manylinux2014_x86_64.whl|
|pyasn1_modules-0.4.2-py3-none-any.whl|
|httplib2-0.31.2-py3-none-any.whl|
|requests_toolbelt-1.0.0-py2.py3-none-any.whl|
|cffi-2.0.0-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.whl|
|proto_plus-1.28.0-py3-none-any.whl|
|typing_extensions-4.15.0-py3-none-any.whl|
|googleapis_common_protos-1.75.0-py3-none-any.whl|
|TIPCommon-2.3.8-py3-none-any.whl|
|cryptography-46.0.7-cp311-abi3-manylinux_2_34_x86_64.whl|
|pycryptodome-3.23.0-cp37-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|
|google_api_core-2.30.3-py3-none-any.whl|
|pyasn1-0.6.3-py3-none-any.whl|


## Actions
#### Add Note And Wait For Reply
Add a note and wait for new notes to be added to the given request.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Request ID|The requests' ID.|True|String||
|Note|The note's content.|True|Content||
|Is Public|Whether to make the note public or not.|False|Boolean|false|



#### Create Alert Request
Create an request related to a Siemplify alert
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Subject|The subject of the request.|True|String||
|Requester|The requester of the request. If not specified, set to the user of the API key.|False|String||
|Status|The status of the request.|False|String||
|Technician|The name of the technician assigned to the request.|False|String||
|Priority|The priority of the request.|False|String||
|Urgency|The urgency of the request.|False|String||
|Category|The category of the request.|False|String||
|Request Template|The template of the request.|False|String||
|Request Type|The type of the request. I.e: Incident, Service Request, etc.|False|String||
|Due By Time (ms)|The due date of the request in milliseconds.|False|String||
|Mode|The mode of the request.|False|String||
|Level|The level of the request.|False|String||
|Site|The site of the request.|False|String||
|Group|The group of the request.|False|String||
|Impact|The impact of the request.|False|String||



#### Ping
Test connectivity to ServiceDesk Plus instance.
Timeout - 600 Seconds



#### Add Note
Add a note to a request
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Request ID|The requests' ID.|True|String||
|Note|The note's content.|True|Content||
|Is Public|Whether to make the note public or not.|False|Boolean|false|



#### Close Request
Close a request
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Request ID|The request's ID.|True|String||
|Comment|Closing comment.|True|String||
|Resolution Acknowledged|Whether the resolution of the request is acknowledged or not.|False|Boolean||



#### Get Request
Retrieve information about a request
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Request ID|The ID of the request.|True|String||



##### JSON Results
```json
{"isvipuser": "No", "subcategory": null, "resolvedtime": "0", "site": "Chicago", "timespentonreq": "0hrs 0min", "technician": "Shawn Adams", "responseduebytime": "1556101814544", "shortdescription": "Testing the API adding request", "fr_duetime": "1556101814544", "subject": "Testing API 2", "impact": "Affects Business", "city": "London", "group": null, "approval_status": null, "area": null, "requesttype": "Convert the Incident to Change", "yettoreplycount": null, "priority": "High", "respondedtime": "0", "asset": null, "createdby": "Demo", "duebytime": "1556164814544", "department": null, "status": "Work Inprogress", "category": "General", "fcr": "false", "description": "Testing the API adding request", "closurecode": null, "workorderid": "123", "completedtime": "0", "requesttemplate": "Default Request", "requester": "Catrin Folkesson", "createdtime": "1556092814544", "technician_loginname": "adams", "editing_status": "0", "level": "Tier 1", "country": "India", "is_catalog_template": "false", "sla": "High SLA", "item": null, "closurecomments": null, "mode": "SMS", "editorid": "null", "impactdetails": null, "urgency": "High"}
```



#### Wait For Field Update
Wait for a field of a request ot update to a desired value.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Request ID|The ID of the request.|True|String|None|
|Field Name|The name of the field to be updated.|True|String|None|
|Values|Desired values for the given field.|True|String|None|



#### Update Request
Update a request
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Request ID|The id of the request to update.|True|String||
|Requester|The requester of the request. If not specified, set to the user of the API key.|False|String||
|Description|The description of the request.|False|String||
|Status|The status of the request.|False|String||
|Technician|The name of the technician assigned to the request.|False|String||
|Priority|The priority of the request.|False|String||
|Urgency|The urgency of the request.|False|String||
|Category|The category of the request.|False|String||
|Request Template|The template of the request.|False|String||
|Request Type|The type of the request. I.e: Incident, Service Request, etc.|False|String||
|Due By Time (ms)|The due date of the request in milliseconds.|False|String||
|Mode|The mode of the request.|False|String||
|Level|The level of the request.|False|String||
|Site|The site of the request.|False|String||
|Group|The group of the request.|False|String||
|Impact|The impact of the request.|False|String||



##### JSON Results
```json
{"isvipuser": "No", "subcategory": null, "resolvedtime": "0", "site": "Chicago", "timespentonreq": "0hrs 0min", "technician": "Shawn Adams", "responseduebytime": "1556101814544", "shortdescription": "Testing the API adding request", "fr_duetime": "1556101814544", "subject": "Testing API 2", "impact": "Affects Business", "city": "London", "group": null, "approval_status": null, "area": null, "requesttype": "Convert the Incident to Change", "yettoreplycount": null, "priority": "High", "respondedtime": "0", "asset": null, "createdby": "Demo", "duebytime": "1556164814544", "department": null, "status": "Work Inprogress", "category": "General", "fcr": "false", "description": "Testing the API adding request", "closurecode": null, "workorderid": "123", "completedtime": "0", "requesttemplate": "Default Request", "requester": "Catrin Folkesson", "createdtime": "1556092814544", "technician_loginname": "adams", "editing_status": "0", "level": "Tier 1", "country": "India", "is_catalog_template": "false", "sla": "High SLA", "item": null, "closurecomments": null, "mode": "SMS", "editorid": "null", "impactdetails": null, "urgency": "High"}
```



#### Wait For Status Update
Wait for the status of a request ot update to a desired status.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Request ID|The ID of the request.|True|String|None|
|Statuses|Desired request statuses, comma separated.|True|String|None|



#### Create Request
Create a new request
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Subject|The subject of the request.|True|String||
|Requester|The requester of the request. If not specified, set to the user of the API key.|False|String||
|Description|The description of the request.|False|String||
|Status|The status of the request.|False|String||
|Technician|The name of the technician assigned to the request.|False|String||
|Priority|The priority of the request.|False|String||
|Urgency|The urgency of the request.|False|String||
|Category|The category of the request.|False|String||
|Request Template|The template of the request.|False|String||
|Request Type|The type of the request. I.e: Incident, Service Request, etc.|False|String||
|Due By Time (ms)|The due date of the request in milliseconds.|False|String||
|Mode|The mode of the request.|False|String||
|Level|The level of the request.|False|String||
|Site|The site of the request.|False|String||
|Group|The group of the request.|False|String||
|Impact|The impact of the request.|False|String||



##### JSON Results
```json
{"isvipuser": "No", "subcategory": null, "resolvedtime": "0", "site": "Chicago", "timespentonreq": "0hrs 0min", "technician": "Shawn Adams", "responseduebytime": "1556101814544", "shortdescription": "Testing the API adding request", "fr_duetime": "1556101814544", "subject": "Testing API 2", "impact": "Affects Business", "city": "London", "group": null, "approval_status": null, "area": null, "requesttype": "Convert the Incident to Change", "yettoreplycount": null, "priority": "High", "respondedtime": "0", "asset": null, "createdby": "Demo", "duebytime": "1556164814544", "department": null, "status": "Work Inprogress", "category": "General", "fcr": "false", "description": "Testing the API adding request", "closurecode": null, "workorderid": "123", "completedtime": "0", "requesttemplate": "Default Request", "requester": "Catrin Folkesson", "createdtime": "1556092814544", "technician_loginname": "adams", "editing_status": "0", "level": "Tier 1", "country": "India", "is_catalog_template": "false", "sla": "High SLA", "item": null, "closurecomments": null, "mode": "SMS", "editorid": "null", "impactdetails": null, "urgency": "High"}
```









