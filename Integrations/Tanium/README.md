
# Tanium

Tanium is a feature-packed endpoint management and endpoint security platform designed to strengthen and optimize an organization’s cybersecurity efforts. The platform gives security teams the tools they need to fortify existing security gaps or completely overhaul their cybersecurity environments, providing complete threat response capabilities from a single endpoint agent. Encompassing everything from asset and threat discovery to complete threat response capabilities from a single endpoint agent, Tanium gives security teams the tools they need to fortify existing security gaps and/or completely overhaul their cyber security environments to adequately prepare themselves for future generations of cyber threats.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|None|True|String||
|API Token|None|True|Password|*****|
|Verify SSL|None|False|Boolean|true|


#### Dependencies
| |
|-|
|chardet-5.2.0-py3-none-any.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|certifi-2024.7.4-py3-none-any.whl|
|idna-3.8-py3-none-any.whl|
|EnvironmentCommon-1.0.0-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|


## Actions
#### Enrich Entities
Enrich entities using information from Tanium. Supported entities: Hostname, IP Address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Additional Fields|Specify additional fields to fetch from Tanium for entity enrichment. Parameter accepts multiple values as a comma separated string.|False|String||



#### List Connections
List endpoint connections in Tanium.
Timeout - 600 Seconds



#### Ping
Test connectivity to the Tanium installation with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Get Task Details
Retrieve details about a task in Tanium. Action works with Tanium Threat Response API. Note: Action is running as async, if "Wait For Completion" is enabled, please adjust script timeout value in Siemplify IDE for action as needed.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Task IDs|Specify a comma-separated list of task ids for which you want to fetch details.|True|String||
|Wait For Completion|If enabled, action will wait for the task to have status "Completed", "Incomplete", "Error".|False|Boolean|true|



#### Delete File
Download a file from endpoints in Tanium. Action works with Tanium Threat Response API. Supported Entities: Hostname, IP Address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File Paths|Specify the absolute path of the files on the endpoint that needs to be deleted.|True|String||



#### Create Connection
Create connection to the endpoint in Tanium. Supported Entities: Hostname, IP Address.
Timeout - 600 Seconds



#### Get Question Results
Fetch results for the Tanium question. Action is a Siemplify async action. Note that the action is not working with Siemplify entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Question ID|Specify Tanium question id to get results for.|True|String||
|Create Case Wall Table|If enabled, action will create a case wall table as part of action results.|False|Boolean|true|
|Max Rows to Return|Specify the max number of rows action should return for the question.|True|String|50|



#### Download File
Download a file from endpoints in Tanium. Action works with Tanium Threat Response API. Supported Entities: Hostname, IP Address. Note: Action is running as async, please adjust script timeout value in Siemplify IDE for action as needed.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File Paths|Specify the absolute path of the files on the endpoint that needs to be downloaded.|True|String||
|Download Folder Path|Specify the path to the folder, where you want to store the files.|True|String||
|Overwrite|If enabled, action will overwrite the file with the same name.|False|Boolean|false|



#### Quarantine Endpoint
Quarantine the endpoints in Tanium. Action works with Tanium Threat Response API. Supported Entities: Hostname, IP Address. Note: Action is running as async, if "Only Initiate" is set to false, please adjust script timeout value in Siemplify IDE for action as needed.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Only Initiate|If enabled, action will only initiate the task execution without waiting for results.|False|Boolean|false|
|Package Names|Specify a JSON object containing all of the package names for each OS.|True|String|{"Linux":"Apply Linux IPTables Quarantine","Mac":"Apply Mac PF Quarantine","Windows":"Apply Windows IPsec Quarantine"}|
|Package Parameters|Specify a JSON object containing all of the parameters for the package being deployed. If nothing is provided, action will use the following payload: [{"key":"$1","value":null},{"key":"$2","value":null},{"key":"$3","value":null},{"key":"$4","value":null},{"key":"$5","value":null},{"key":"$6","value":null},{"key":"$7","value":null},{"key":"$8","value":null},{"key":"$9","value":null}]|False|String||



#### List Endpoint Events
List events related to the endpoints from Tanium. Action works with Tanium Threat Response API. Supported Entities: Hostname, IP Address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Event Type|Specify the type of the event that needs to be returned.|False|List|Combined|
|Time Frame|Specify a time frame for the results. If "Alert Time Till Now" is selected, action will use start time of the alert as start time for the search and end time will be current time. If "30 Minutes Around Alert Time" is selected, action will search the alerts 30 minutes before the alert happened till the 30 minutes after the alert has happened.  Same idea applies to "1 Hour Around Alert Time" and "5 Minutes Around Alert Time". If "Custom" is selected, you also need to provide "Start Time".|False|List|Last Hour|
|Start Time|Specify the start time for the results. This parameter is mandatory, if "Custom" is selected for the "Time Frame" parameter. Format: ISO 8601|False|String||
|End Time|Specify the end time for the results. Format: ISO 8601. If nothing is provided and "Custom" is selected for the "Time Frame" parameter then this parameter will use current time.|False|String||
|Sort Field|Specify what parameter should be used for sorting.|False|String|timestamp|
|Sort Order|Specify the order of sorting.|False|List|ASC|
|Max Events To Return|Specify how many events to return per entity. Default: 50. Maximum: 500.|False|String|50|



#### Create Question
Create a new Tanium question based on the specified parameters, and the question is immediately asked. Action returns question id that can be passed to “Get Question Results” action to get question results. Note that the action is not working with Siemplify entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Question Text|Specify the contents of Tanium question. Example: Get Operating System from all machines|True|String||









