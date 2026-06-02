
# EasyVista

Radically simplify and accelerate service creation, deployment, and support with  proven and integrated ITSM platform.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|None|True|URL|https://try.easyvista.com/api/v1/|
|Account ID|None|True|String||
|Username|None|True|String||
|Password|None|True|Password|*****|
|Verify SSL|None|False|Boolean||


#### Dependencies
| |
|-|
|charset_normalizer-3.3.2-py3-none-any.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|
|chardet-5.2.0-py3-none-any.whl|
|idna-3.8-py3-none-any.whl|
|certifi-2024.8.30-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|


## Actions
#### Ping
Test connectivity to the EasyVista instance with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Get EasyVista Ticket
Get information on specific EasyVista ticket. Note: action is not working on Siemplify entities, ticket identifier (rfc_number) should be provided.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Ticket Identifier|EasyVista ticket identifier to get info for, eg S201001_000001.|True|String||



#### Add Comment to Ticket
Add a comment to the EasyVista ticket. Note: action is not working on Siemplify entities, action input parameters should be provided.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Ticket Identifier|EasyVista ticket identifier to get info for, eg S201001_000001.|True|String||
|Comment|Comment to add to EasyVista ticket.|True|String||



#### Close EasyVista Ticket
Close EasyVista ticket based on the provided parameters. Note: action is not working on Siemplify entities, ticket identifier (rfc_number) should be provided.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Ticket Identifier|EasyVista ticket identifier, eg S201001_000001.|True|String||
|Comment|Comment explaining the closing of the ticket.|False|String||
|Actions Close Date|Closing date of open actions associated with the ticket and the anticipated closure action. Date should be in the following format: MM/DD/YYYY HH:MM:SS. If the wrong format is provided, action will use current datetime as close date.|False|String||
|Delete ongoing actions?|Specify whether to delete the ticket's ongoing actions on ticket closing.|False|Boolean|False|



#### Wait for the Ticket Update
Action pauses the playbook execution and periodically connects to EasyVista until timeout and checks if the specified ticket got an update. Action also can monitor specific field for the update, once that field is updated - action completes and fetches back the updated ticket information. 
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Ticket Identifier|EasyVista ticket identifier, eg S201001_000001.|True|String||
|Field To Monitor|EasyVista ticket field to monitor for the update.|False|List|Status|









