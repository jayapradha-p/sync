
# SumoLogicCloudSIEM

Sumo Logic Cloud SIEM provides threat detection and incident response for modern IT environments such as hybrid, multi-cloud, and microservices. Whether you’re looking for your first cloud SIEM, replacing your legacy SIEM, looking for an add-on solution to monitor cloud workloads, or seeking to consolidate your SIEM tools, Sumo Logic is the leading solution in the market.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|API root of the Sumo Logic Cloud SIEM instance.|True|String|https://{instance}|
|API Key|API Key of the Sumo Logic Cloud SIEM account. Note: API key has priority over other authentication method.|False|Password|*****|
|Access ID|Access ID of the Sumo Logic Cloud SIEM account. Note: both Access ID and Access Key are required for this type of authentication.|False|String||
|Access Key|Access Key of the Sumo Logic Cloud SIEM account. Note: both Access ID and Access Key are required for this type of authentication.|False|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Sumo Logic Cloud SIEM server is valid.|False|Boolean|true|


#### Dependencies
| |
|-|
|beautifulsoup4-4.12.3-py3-none-any.whl|
|certifi-2026.4.22-py3-none-any.whl|
|soupsieve-2.8.3-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|bs4-0.0.2-py2.py3-none-any.whl|
|EnvironmentCommon-1.0.1-py2.py3-none-any.whl|
|python_dateutil-2.8.2-py2.py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|TIPCommon-1.0.11-py2.py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|idna-3.13-py3-none-any.whl|
|six-1.17.0-py2.py3-none-any.whl|


## Actions
#### Add Comment To Insight
Add a comment to insight in Sumo Logic Cloud SIEM.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Insight ID|Specify the ID of the insight to which action needs to add a comment.|True|String||
|Comment|Specify the comment that needs to be added in insight.|True|String||



#### Add Tags To Insight
Add tags to insight in Sumo Logic Cloud SIEM.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Insight ID|Specify the ID of the insight to which action needs to add tags.|True|String||
|Tags|Specify a comma-separated list of tags that needs to be added in insight.|True|String||



#### Update Insight
Update insight status in Sumo Logic Cloud SIEM.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Insight ID|Specify the ID of the insight needs to be updated.|True|String||
|Status|Specify what status to set for the insight.|True|List|Select One|
|Assignee Type|Specify the assignee type for the "Assignee" parameter.|True|List|User|
|Assignee|Specify the assignee identifier.|False|String||



#### Enrich Entities
Enrich entities using information from Sumo Logic Cloud SIEM. Supported entities: Hostname, User, IP address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Create Insight|If enabled, action will create an insight containing all of the retrieved information about the entity.|False|Boolean|true|



#### Ping
Test connectivity to the Sumo Logic Cloud SIEM with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Search Entity Signals
Search signals related to entities in Sumo Logic Cloud SIEM. Supported entities: IP Address, Hostname, Username.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Lowest Severity To Return|Specify the lowest severity number that will be used to return signals. Maximum: 10.|False|String|5|
|Time Frame|Specify a time frame for the results. If "Custom" is selected, you also need to provide "Start Time". If "30 Minutes Around Alert Time" is selected, action will search the alerts 30 minutes before the alert happened till the 30 minutes after the alert has happened.  Same idea applies to "1 Hour Around Alert Time" and "5 Minutes Around Alert Time".|False|List|Last Hour|
|Start Time|Specify the start time for the results. This parameter is mandatory, if "Custom" is selected for the "Time Frame" parameter. Format: ISO 8601|False|String||
|End Time|Specify the end time for the results. Format: ISO 8601. If nothing is provided and "Custom" is selected for the "Time Frame" parameter then this parameter will use current time.|False|String||
|Max Signals To Return|Specify how many signals to return per entity. Default: 50.|False|String|50|









## Connectors
#### Sumo Logic Cloud SIEM - Insights Connector
Pull information about insights from Sumo Logic Cloud SIEM. Note: dynamic list filter works with "name" parameter.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|API Root|API root of the Sumo Logic Cloud SIEM instance.|True|String|https://{instance}|
|API Key|API Key of the Sumo Logic Cloud SIEM account. Note: API key has priority over other authentication method.|False|Password|*****|
|Access ID|Access ID of the Sumo Logic Cloud SIEM account. Note: both Access ID and Access Key are required for this type of authentication.|False|String||
|Access Key|Access Key of the Sumo Logic Cloud SIEM account. Note: both Access ID and Access Key are required for this type of authentication.|False|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Sumo Logic Cloud SIEM server is valid.|False|Boolean|true|
|Lowest Severity To Fetch|Lowest severity that needs to be used to fetch insights. Possible values: Low, Medium, High, Critical. If nothing is specified, the connector will ingest insights with all severities.|False|String||
|Max Hours Backwards|Number of hours before the first connector iteration to retrieve insights from. This parameter applies to the initial connector iteration after you enable the connector for the first time, or used as a fallback value in cases where connector's last run timestamp expires.|False|Int|1|
|Max Insights To Fetch|How many insights to process per one connector iteration. Default: 20.|False|Int|20|
|Use dynamic list as a blacklist|If enabled, dynamic lists will be used as a blacklist.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




