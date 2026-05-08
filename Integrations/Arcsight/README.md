
# Arcsight

Real-time threat detection and automated response backed by a powerful, open, and intelligent SIEM (Security Information and Event Management).

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root|None|True|String||
|Username|None|True|String||
|Password|None|True|Password||
|CA Certificate File|None|False|String||
|Verify SSL|None|False|Boolean||


#### Dependencies
| |
|-|
|certifi-2024.7.4-py3-none-any.whl|
|TIPCommon-1.0.16-py2.py3-none-any.whl|
|netaddr-1.3.0-py3-none-any.whl|
|idna-3.7-py3-none-any.whl|
|simplejson-3.19.2-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl|
|requests-2.32.3-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|
|EnvironmentCommon-1.0.2-py2.py3-none-any.whl|
|charset_normalizer-3.3.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|


## Actions
#### Add Entities To Active List
Add entities to the active list in ArcSight.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Active List Name|Specify the name of the active list to which you want to add entities.|True|None||
|Entity Column|Specify the name of the column, where entity value should be put.|True|None||
|Additional Fields|Specify additional fields that should be added alongside the entity in the active list. Format is a JSON object. Example: {"Column_1": "Value_1","Column_2": "Value_2"}|False|None||



#### Add Entries To Activelist
Add new entry to active list in ArcSight. Column values are separated by delimiter ‘|' and entries are separated by ‘;’ in parameter ‘Entries’. Column names are separated by delimiter ‘;’ in parameter ‘Columns’. You can also use Entries JSON instead of ‘Columns’ + 'Entries’“.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Columns|Specify the name of the columns, where you want to put values for the entries. Format: Column_name1;Column_name2|False|None||
|Entries|Specify the entries. Format entry1_value1|entry1_value2;entry2_value1|entry2_value2|False|None||
|Active List UUID|Specify the UUID of the active list, where you want to add new entries. Note: parameter “Active list UUID“ takes priority over “Active list name“. Example: HLZRc9yYBABC-lHtlf3-f0Q==|False|None||
|Active list name|Specify the name of the active list, where you want to add new entries. Note: parameter “Active list UUID“ takes priority over “Active list name“.|False|None||
|Entries JSON|Specify a list of JSON objects that contain information about the entry. Note: Combination of ‘Columns' and ‘Entries’ parameters have priority over 'Entries JSON’. Format: [{"Column_1": "Value_1", "Column_2": "Value_2"}, {"Column_1": "Value_3", "Column_2": "Value_4"}]|False|None||



#### Change Case Stage
Update the stage of the case in ArcSight.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Case Name|Specify the name of the case for which you want to update the stage.|True|None||
|Stage|Specify a new stage for the case. Possible values: INITIAL, QUEUED, CLOSED, FINAL, and FOLLOW_UP.|True|None||



#### Get Activelist Entries
Retrieve active list entries in ArcSight
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Active list UUID|Specify the UUID of the active list for which you want to retrieve entries. Note: parameter “Active list UUID“ takes priority over “Active list name“. Example: HLZRc9yYBABC-lHtlf3-f0Q==|False|None||
|Active list name|Specify the name of the active list for which you want to retrieve entries. Note: parameter “Active list UUID“ takes priority over “Active list name“.|False|None||
|Map Columns|If enabled, action will map columns to the values in the JSON result.|False|None||
|Max Entries To Return|Specify how many entries to return.|False|None||



#### Get Query Results
Get results for the provided query in ArcSight
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Query ID|Specify the ID of the query for which you want to return results. Note: parameter “Query ID“ takes priority over “Query Name“. Example: cyUJKRz4BABCFwS9iFPq+aA==|False|None||
|Max Items To Return|Specify how many items to return in the response.|False|None||
|Query Name|Specify the name of the query for which you want to return results. Note: parameter “Query ID“ takes priority over “Query Name“.|False|None||



#### Get Report
Get details about report in ArcSight.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Report Full Path (URI)|Specify the URI to the report. Example: /All Reports/ArcSight Foundation/MITRE ATT&CK/Mitre ATT&CK Summary|True|None||
|Field 2|The dynamic fields for the query to generate the report|False|None||
|Field 3|The dynamic fields for the query to generate the report|False|None||
|Field 4|The dynamic fields for the query to generate the report|False|None||
|Field 5|The dynamic fields for the query to generate the report|False|None||
|Field 6|The dynamic fields for the query to generate the report|False|None||
|Field 7|The dynamic fields for the query to generate the report|False|None||
|Field 8|The dynamic fields for the query to generate the report|False|None||
|Field 9|The dynamic fields for the query to generate the report|False|None||
|Field 10|The dynamic fields for the query to generate the report|False|None||



#### Is Value In Activelist Column
Action checks, if entities were found in ArcSight Activelist
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Active list UUID|Specify the UUID of the active list, where you want to search for entities. Note: parameter “Active list UUID“ takes priority over “Active list name“. Example: HLZRc9yYBABC-lHtlf3-f0Q==|False|None||
|Column name|Specify the name of the column, where you want to search for the entity.|True|None||
|Active list name|Specify the name of the active list, where you want to search for entities. Note: parameter “Active list UUID“ takes priority over “Active list name“.|False|None||



#### List Resources
List available queries in ArcSight.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Return Active Lists|If enabled, action will return available active lists.|False|None||
|Return Queries|If enabled, action will return available queries|False|None||
|Return Cases|If enabled, action will return available cases.|False|None||
|Return Reports|If enabled, action will return available reports.|False|None||
|Max Resources To Return|Specify how many resources to return per type.|False|None||



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Search
Search for available resources in ArcSight
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Search Query|Specify the search query.|True|None||
|Max Items To Return|Specify how many items to return in the response.|False|None||









## Connectors
#### ArcSight - Security Events Connector
Pull correlations from ArcSight. Note: dynamic list works with "name" parameter. Please refer to the doc portal for the configuration setup. This connector is suitable for Saas deployment of Chronicle SOAR and is the recommended one for production use.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|None||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|None|.*|
|API Root|API root of the ArcSight instance.|True|None|https://{ip}|
|Username|Username of the ArcSight account.|True|None||
|Password|Password of the ArcSight account.|True|None||
|Report Name|Name of the report that will be used to fetch events.|True|None||
|Fetch Base Events|If enabled, connector will also fetch base events.|False|None|true|
|Lowest Priority To Fetch|Lowest priority that will be used to fetch events. Possible values are in range 1 to 10. If nothing is provided, all events will be ingested.|False|None||
|Max Events To Fetch|How many alerts to process per one connector iteration. Maximum is 1000.|False|None|100|
|Use dynamic list as a blocklist|If enabled, dynamic lists will be used as a blocklist.|False|None|false|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the ArcSight server is valid.|False|None|false|
|Proxy Server Address|The address of the proxy server to use.|False|None||
|Proxy Username|The proxy username to authenticate with.|False|None||
|Proxy Password|The proxy password to authenticate with.|False|None||


#### Arcsight ESM Connector
Arcsight ESM Connector

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Server Address|Server address of the ArcSight instance|True|None|None|
|Username|Username of the ArcSight account|True|None|None|
|Password|Password of the ArcSight account|True|None|None|
|Events Count Limit|How many events to process per one alert|True|None|15|
|Cases Folder Path|Absolute path to cases. Example: /opt/Correlations|True|None|/opt/Correlations|
|Alerts Count Limit|How many alerts to process per one iteration|True|None|10|
|Environment Field Name|The name of the environment's field. e.g. event.CustomerURI|True|None|event.CustomerURI|
|Secondary Device Product Field|Secondary field for Device Product|False|None|None|
|Alert Custom Fields Names|Additional fields that should be added to Siemplify Alert. Example: source_address|False|None|None|
|Done files retention days|For how many days to leave files in the “Done” folder |True|None|3|
|Error files retention days|For how many days to leave files in the “Error” folder|True|None|14|
|Proxy Server Address|The address of the proxy server to use.|False|None|None|
|Proxy Username|The proxy username to authenticate with.|False|None|None|
|Proxy Password|The proxy password to authenticate with.|False|None|None|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the ArcSight ESM server is valid.|False|None|false|
|CA Certificate File|Base 64 encoded CA certificate file.|False|None||




