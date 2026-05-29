
# Bitdefender GravityZone

Bitdefender Control Center API's allow developers and SOC's to automate business workflows. Docs: https://github.com/snags141/SiemplifyIntegration_BitdefenderGravityZone

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Key|API Key generated under "My Account"|True|Password|*****|
|Access URL|Access URL for Control Center API|True|String|https://cloud.gravityzone.bitdefender.com/api|
|Verify SSL|Verify SSL when making requests|False|Boolean|false|


#### Dependencies
| |
|-|
|urllib3-2.5.0-py3-none-any.whl|
|charset_normalizer-3.4.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|
|requests-2.32.4-py3-none-any.whl|
|idna-3.10-py3-none-any.whl|
|certifi-2025.6.15-py3-none-any.whl|


## Actions
#### Blocklist - Add Hashes
Use this method to add one or more file hashes to the Blocklist. Hashes supported: SHA256, MD5.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Hash List|A comma-separated list of SHA256 or MD5 hashes.|True|String|hash1,hash2|
|Source Info|A description for the hashes.|True|String|Determined to be malicious.|



#### Create Scan Task
This method creates a task to isolate the specified endpoint.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Task Name|The name of the task. If the parameter is not passed, the name will be automatically generated.|False|String|None|
|Target IDs|A list with the IDs of the targets to scan. The target ID can designate an endpoint or a container.|True|String|targetId1,targetId2|
|Scan Type|The type of scan. Available options are: 1 - quick scan; 2 - full scan; 3 - memory scan; 4 - custom scan|True|List|Quick|
|Custom Scan - Depth|The scan profile. Available options: 1 - aggressive; 2 - normal; 3 - permissive. This parameter is only used when scan type is Custom|False|List|Normal|
|Custom Scan - Paths|Comma-separated list of target paths to be scanned. This parameter is only used when scan type is Custom|False|String|LocalDrives|



#### Blocklist - List Items
This method lists all the hashes that are present in the blocklist.
Timeout - 600 Seconds



#### Get Hourly Usage for EC2 Instances
This method exposes the hourly usage for each Amazon instance category (micro, medium etc.).
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Target Month|The month for which the usage is returned. The month will be provided in the following format: mm/yyyy. The default value is the current month.|True|String|01/2020|



#### Blocklist - Remove Item
This method removes an item from the Blocklist, identified by its ID
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Hash ID|The ID of the item in the Blocklist to be deleted|True|String|Eg: 0df7568c-59c1-48e0-a31b-18d83e6d9810|



#### Isolate Endpoint
This method creates a task to isolate the specified endpoint.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Endpoint ID|The ID of the endpoint for which the details will be returned|True|String|oBFA8Ie3Oh4iXCtyr5Z9iw|



#### Ping

Timeout - 600 Seconds



#### Policies - List All
This method retrieves the list of available policies.
Timeout - 600 Seconds



#### Get Custom Groups List
This method retrieves the list of groups under a specified group.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Parent ID|Parent group ID for which the child groups will be listed. 'Computers and Groups' and 'Deleted' groups are returned if the passed parameter is null.|False|String||



#### Quarantine - Remove Items
This method creates a new task to remove items from quarantine.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Service|Allowed services are: computers, for "Computers and Virtual Machines" or exchange, for "Security for Exchange"|True|List|Computers|
|Quarantine Item IDs|Comma-separated list of quarantine items IDs. The maximum number of items that can be removed once is 100.|True|String|itemId1,itemId2|



#### Reports - Get Download Links
This method returns an Object with information regarding the report availability for download and the corresponding download links.
The instant report is created one time only and available for download for less than 24 hours.
Scheduled reports are generated periodically and all report instances are saved in the GravityZone database.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Report ID|The report ID to fetch|True|String|reportId|



#### Reports - List All
This method returns the list of scheduled reports, according to the parameters received.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Report Name|The name of the report.|False|String|None|
|Report Type|The report type.|False|List||



#### Get Network Inventory Items
This method returns network inventory items. Note - Some filters require a specific license to be active, otherwise they are ignored, resulting in an inaccurate API response. The field name works with partial matching.
The filter returns the items whose names are exact match or start with the specified value. To use the specified value as a suffix, use the asterisk symbol (*).
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Filter - Name|A string for filtering the items by name. Minimum required string length is three characters.|False|String|None|
|Filter - MAC Addresses|Comma-separated list of MAC addresses used to filter the endpoints regardless of their protection status.|False|String|None|
|Filter - SSID|The SSID (Active Directory SID of the endpoint) used to filter the endpoints regardless of their protection status.|False|String|None|
|Filter - Depth - All Items Recursively|Boolean to filter all endpoints recursively within the Network Inventory of a company.|False|Boolean|false|
|Filter - Security Servers|Boolean to filter all Security Servers|False|Boolean|false|
|Filter - Managed Relays|Boolean to filter all endpoints with Relay role. |False|Boolean|false|
|Filter - Managed Exchange Servers|Boolean to filter all protected Exchange servers.|False|Boolean|false|
|Filter - Managed with BEST|Boolean to filter all endpoints with the security agent installed on them.|False|Boolean|false|
|Filter - Virtual Machines|Boolean to filter all virtual machines.|False|Boolean|false|
|Filter - Computers|Boolean to filter all computers.|False|Boolean|false|
|Filter - EC2 Instances|Boolean to filter all Amazon EC2 Instances.|False|Boolean|false|
|Filter - Groups|Boolean to filter all custom groups of endpoints.|False|Boolean|false|
|Parent ID|The ID of the container for which the network items will be returned.|False|String|None|



#### Get Scan Tasks List
This method returns the list of scan tasks.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Task Status|The status of the task.|True|List|All|
|Task Name|Use an asterisk in front to search its appearance anywhere in the name. If omitted, only returns results where the name starts with the keyword|False|String|None|



#### Policies - Get Details
This method retrieves all information related to a security policy.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Policy ID|The ID of the policy to be queried.|True|String|5e1023820d21ea80605bf919|



#### Quarantine - Add File
This method creates a new task to add a file to quarantine.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File Path|The absolute file path on disk. This can be at most 4096 characters in length and should have the format suitable to the target's operating system.|True|String|C:\Users\Public\malicious.exe|
|Endpoint IDs|A list with the IDs of the target endpoints. Max 100 targets at once. Only endpoints having the EDR Sensor module active are considered valid targets.|True|String|targetId1,targetId2|



#### Quarantine - Get Items List
This method retrieves the list of quarantined items available for a company. An item can be a file or an Microsoft Exchange object.
The filter fields Threat Name, File Path, and IP Address work with partial matching.
The filter returns the items which are exact match or start with the specified value.
To use the specified value as a suffix, use the asterisk symbol (*). For example:
If filePath is C:\temp, the API returns all items originating from this folder, including sub-folders.
If filePath is *myfile.exe, then the API returns a list of all myfile.exe files from anywhere on the system.
The Exchange filters require a valid license key for Security for Exchange.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Service|Allowed services are: computers, for "Computers and Virtual Machines" or exchange, for "Security for Exchange"|True|List|Computers|
|Filter - Threat Name|Filters the quarantined items by threat name.This filter is available for computers and exchange services.|False|String|None|
|Filter - Start Date|Filters the items that quarantined after the specified date. Format for startDate is in ISO 8601.The filter is available for computers and exchange.|False|String|None|
|Filter - End Date|Filters the items quarantined before the specified date.Format for startDate is in ISO 8601.The filter is available for computers and exchange.|False|String|None|
|Filter - File Path|Filters the quarantined items by file path. This filter is available for computers service.|False|String|None|
|Filter - IP Address|Filters the quarantine items by IP address. This filter is available for computers service.|False|String|None|
|Filter - Action Status|Filters the quarantine items by action status. "Pending Save" Is only available to the Exchange Service.|False|List|None|
|Endpoint ID|ID of the computer for which you want to retrieve the quarantined items. If not passed, he method returns the items quarantined in the entire network.|False|String|None|



#### Quarantine - Restore Exchange Items
This method creates a new task to restore items from the quarantine for Exchange Servers.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|EWS URL|The Exchange Web Services URL .The EWS URL is necessary when the Exchange Autodiscovery does not work.|False|String|None|
|Email|The email address of the Exchange user. This parameter is necessary when the email address is different from the username.|False|String|None|
|Password|The password of an Exchange user|True|Password|*****|
|Username|The username of an Microsoft Exchange user. The username must include the domain name.|True|String|username|
|Quarantine Item IDs|Comma-separated list of quarantine items IDs. The maximum number of items that can be removed once is 100.|True|String|itemId1,itemId2|



#### Quarantine - Restore Items
This method creates a new task to restore items from the quarantine.

Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Location to Restore|The absolute path to the folder where the items will be restored. If the parameter is not set, the original location will be used.|False|String|None|
|Quarantine Item IDs|Comma-separated list of quarantine items IDs. The maximum number of items that can be removed once is 100.|True|String|itemId1,itemId2|
|Service|Allowed services are: computers, for "Computers and Virtual Machines" or exchange, for "Security for Exchange"|True|List|Computers|
|Add Exclusion in Policy|Exclude the files to be restored from future scans. Exclusions do not apply to items with the Default Policy assigned.|False|Boolean|false|



#### Restore Isolated Endpoint
This method creates a task to restore the specified endpoint from isolation.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Endpoint ID|The ID of the endpoint for which the details will be returned|True|String|oBFA8Ie3Oh4iXCtyr5Z9iw|



#### Get Endpoints List
Get list of endpoints
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Filter - SSID|The SSID (Active Directory SID of the endpoint) used to filter the endpoints regardless of their protection status.|False|String|None|
|Filter - Depth - All Items Recursively|Boolean to filter all endpoints recursively within the Network Inventory of a company.|False|Boolean|false|
|Filter - Security Servers|Boolean to filter all Security Servers|False|Boolean|false|
|Filter - Managed Relays|Boolean to filter all endpoints with Relay role. |False|Boolean|false|
|Filter - Managed Exchange Servers|Boolean to filter all protected Exchange servers.|False|Boolean|false|
|Parent ID|The ID of the target company or group. If not specified or set with a company ID, the method returns only the endpoints under Computers and Groups.|False|String|None|
|Endpoints|Select whether to return only managed endpoints, unmanaged endpoints, or all endpoints.|True|List|All|
|Filter - Managed with BEST|Boolean to filter all endpoints with the security agent installed on them.|False|Boolean|false|
|Filter - Name|A string for filtering the items by name. Minimum required string length is three characters.|False|String|None|
|Filter - MAC Addresses|Comma-separated list of MAC addresses used to filter the endpoints regardless of their protection status.|False|String|None|



#### Get Managed Endpoint Details
This method returns detailed information, such as: details to identify the endpoint and the security agent, the status of installed protection modules.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Endpoint ID|The ID of the endpoint for which the details will be returned|True|String|oBFA8Ie3Oh4iXCtyr5Z9iw|



#### Set Endpoint Label
This method sets a new label to an endpoint.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Label|A string representing the label. The maximum allowed length is 64 characters. Enter an empty string to reset a previously set label.|True|String|Some label|
|Endpoint ID|The ID of the endpoint for which the details will be returned|True|String|oBFA8Ie3Oh4iXCtyr5Z9iw|



#### Create Scan Task by MAC Address
Use this method to generate a scan task for managed endpoints identified by their MAC address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|MAC Addresses|The list of mac addresses of the endpoints to be scanned. You can specify at most 100 MAC addresses at once|True|String|macaddr1,macaddr2|
|Scan Type|The type of scan. Available options are: 1 - quick scan; 2 - full scan; 3 - memory scan; 4 - custom scan|True|List|Quick|
|Task Name|The name of the task. If the parameter is not passed, the name will be automatically generated.|False|String|None|
|Custom Scan - Depth|The scan profile. Available options: 1 - aggressive; 2 - normal; 3 - permissive. This parameter is only used when scan type is Custom|False|List|Normal|
|Custom Scan - Paths|Comma-separated list of target paths to be scanned. This parameter is only used when scan type is Custom|False|String|LocalDrives|









