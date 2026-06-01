
# SysAid

SysAid is an IT service management solution that offers all the ITIL essentials. It's everything you need for easy and efficient ITSM in a single tool.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root|None|True|String|https://{account}.sysaidit.com/api/v1|
|Username|None|True|String||
|Password|None|True|Password|*****|
|Verify SSL|None|False|Boolean||



## Actions
#### Ping
Test SysAid connectivity.
Timeout - 600 Seconds



#### Get Service Request
Get a service request.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Service Request ID|The ID of the service request to get info about.|True|String||



#### Close Service Request
Close a service request.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Service Request ID|The ID of the service request to delete.|True|String||
|Solution|The solution of the request service.|True|String||



#### List Service Requests
List service requests.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Service Request Type|The type of the service request to filter by. Valid values: incident, request, problem, change, all.|False|String||
|Status|The status of the request service to filter by.|False|String||
|Priority|The priority of the request service to filter by.|False|String||
|Assignee|The assignee of the request service to filter by.|False|String||
|Urgency|The urgency of the request service to filter by.|False|String||
|Request User|The request user of the request service to filter by.|False|String||
|Category|The category of the request service to filter by.|False|String||
|Subcategory|The subcategory of the request service to filter by.|False|String||
|Third Category|The third category of the request service to filter by.|False|String||
|Assigned Group|The assigned group of the request service to filter by.|False|String||
|Get Archived|Whether to get archived request services or not.|False|Boolean||



#### Create Service Request
Create a service request.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Title|The title of the service request.|True|String||
|Description|The description of the service request.|True|String||
|Service Request Type|The type of the service request. Valid values: incident, request, problem, change, all.|False|String||
|Status|The status of the request service.|True|String||
|Priority|The priority of the request service.|True|String||
|Assignee|The assignee of the request service.|True|String||
|Urgency|The urgency of the request service.|True|String||
|Request User|The request user of the request service.|False|String||
|Category|The category of the request service.|False|String||
|Subcategory|The subcategory of the request service.|False|String||
|Third Category|The third category of the request service.|False|String||
|Assigned Group|The assigned group of the request service.|False|String||



#### List Users
List SysAid users.
Timeout - 600 Seconds



#### Delete Service Request
Delete a service request.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Service Request ID|The ID of the service request to delete.|True|String||



#### Update Service Request
Update a service request.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Service Request ID|The id of the service request to update.|True|String||
|Status|The new status of the request service.|False|String||
|Priority|The new priority of the request service.|False|String||
|Assignee|The new assignee of the request service.|False|String||
|Urgency|The new urgency of the request service.|False|String||
|Request User|The new request user of the request service.|False|String||
|Category|The new category of the request service.|False|String||
|Subcategory|The new subcategory of the request service.|False|String||
|Third Category|The new third category of the request service.|False|String||
|Assigned Group|The new assigned group of the request service.|False|String||









