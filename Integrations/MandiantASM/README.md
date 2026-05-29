
# MandiantASM

Mandiant Advantage Attack Surface Management automates external asset discovery and analysis to uncover vulnerabilities, misconfigurations and exposures.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|API root of the Mandiant ASM instance. Note: if you want to authenticate with GTI credentials provide "https://www.virustotal.com" as API Root.|True|String|https://asm-api.advantage.mandiant.com|
|Access Key|API Access Key of the Mandiant ASM account|False|String||
|Secret Key|API Secret Key of the Mandiant ASM account.|False|Password|*****|
|GTI API Key|Google Threat Intelligence API Key. Note: API Root should be "https://www.virustotal.com" to use this authentication. GTI API Key authentication has priority over other authentication.|False|Password|*****|
|Project Name|Project name that should be used in Mandiant ASM. If Access Key & Secret Key is used for authentication, this parameter is mandatory.|False|String||
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Mandiant ASM server is valid.|False|Boolean|true|


#### Dependencies
| |
|-|
|TIPCommon-1.0.16-py2.py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|EnvironmentCommon-1.0.2-py2.py3-none-any.whl|
|idna-3.8-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|
|certifi-2024.8.30-py3-none-any.whl|


## Actions
#### Update Issue
Update an issue in Mandiant ASM.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Issue ID|Specify the ID of the issue that needs to be updated.|True|String|None|
|Status|Specify what status to set for the issues.|True|List|Select One|



#### Ping
Test connectivity to the MandiantASM with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Get ASM Entity Details
Return information about a Mandiant ASM entity.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Entity IDs|Specify a comma-separated list of entity IDs for which you want to fetch details.|True|String|None|



#### Search Issues
Search Issues that match the specified criteria in the action Parameters.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Issue IDs|Specify a comma-separated list of issue ids, for which you want to return details.|False|String|None|
|Entity IDs|Specify a comma-separated list of entity ids for which you want to find related issues.|False|String|None|
|Entity Name|Specify a comma-separated list of entity names for which you want to find related issues.|False|String|None|
|Time Parameter|Specify what parameter should be used for filtering time.|False|List|First Seen|
|Time Frame|Specify a time frame for the issues. If “Custom” is selected, you also need to provide “Start Time”.|False|List|Last Hour|
|Start Time|Specify the start time for the results. This parameter is mandatory, if “Custom” is selected for the “Time Frame” parameter. Format: ISO 8601|False|String|None|
|End Time|Specify the end time for the results. Format: ISO 8601. If nothing is provided and “Custom” is selected for the “Time Frame” parameter then this parameter will use current time.|False|String|None|
|Lowest Severity To Return|Specify the lowest severity that should be used to return the issues. If “Select One” is selected, this filter is not applied during the search.|False|List|Select One|
|Status|Specify the status filter for the search. If “Select One” is selected, this filter is not applied during the search.|False|List|Select One|
|Tags|Specify a comma-separated list of tag names, which should be used, when searching for the issues.|False|String|None|
|Max Issues To Return|Specify how many issues to return. Default: 50. Maximum is 200.|False|String|50|



#### Search ASM Entities
Search entities in Mandiant ASM.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Entity Name|Specify a comma-separated list of entity names for which you want to find entities.|False|String|None|
|Critical or High Issue|Specify whether to include only entities with High or Critical Issues.|False|Boolean|false|
|Minimum Vulnerabilities Count|Specify how many vulnerabilities should be related to the entity for it to be returned.|False|String||
|Minimum Issues Count|Specify how many issues should be related to the entity for it to be returned.|False|String||
|Tags|Specify a comma-separated list of tag names, which should be used, when searching for the entities.|False|String|None|
|Max Entities To Return|Specify how many entities to return. Default: 50. Maximum is 200.|False|String|50|









## Connectors
#### Mandiant ASM - Issues Connector
Pull information about issues from Mandiant ASM. Note: The Dynamic List filter works with the "category" parameter.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|API Root|API root of the Mandiant ASM instance. Note: if you want to authenticate with GTI credentials provide “https://www.virustotal.com” as API Root.|True|String|https://asm-api.advantage.mandiant.com|
|Access Key|API Access Key of the Mandiant ASM account.|False|Password|*****|
|Secret Key|API Secret Key of the Mandiant ASM account.|False|Password|*****|
|GTI API Key|Google Threat Intelligence API Key. Note: API Root should be “https://www.virustotal.com” to use this authentication. GTI API Key authentication has priority over other authentication.|False|Password|*****|
|Project Name|Project name that should be used in Mandiant ASM.  If Access Key & Secret Key is used for authentication, this parameter is mandatory.|False|String||
|Lowest Severity To Fetch|Lowest severity that needs to be used to fetch issues. Possible values: Informational, Low, Medium, High, Critical. If nothing is specified, the connector will ingest issues with all severities.|False|String||
|Max Hours Backwards|Number of hours before the first connector iteration to fetch issues from. This parameter applies to the initial connector iteration after you enable the connector for the first time, or used as a fallback value in cases where connector's last run timestamp expires.|False|Int|1|
|Max Issues To Fetch|Specify the number of issues to process per one connector iteration. Default: 10.|False|Int|10|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Mandiant ASM server is valid.|False|Boolean|true|
|Use dynamic list as a blocklist|If enabled, dynamic lists will be used as a blocklist.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




