
# FortiAnalyzer

FortiAnalyzer provides a solution to address current difficulties and strengthen security posture. As an integrated solution, FortiAnalyzer reduces the challenges of supporting multiple point products. It is also designed to include broad visibility and control of an organization’s entire digital attack surface to minimize risk.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|API root of the FortiAnalyzer instance.|True|String|https://{ip_address}|
|Username|Username of the FortiAnalyzer account.|True|String||
|Password|Password of the FortiAnalyzer account.|True|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the FortiAnalyzer is valid.|False|Boolean|true|


#### Dependencies
| |
|-|
|charset_normalizer-3.3.2-py3-none-any.whl|
|idna-3.7-py3-none-any.whl|
|TIPCommon-1.0.12-py2.py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|
|EnvironmentCommon-1.0.1-py2.py3-none-any.whl|
|chardet-5.2.0-py3-none-any.whl|
|certifi-2024.7.4-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|


## Actions
#### Add Comment To Alert
Add a comment to alert in FortiAnalyzer.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Alert ID|Specify the ID of the alert that needs to be updated.|True|String||
|Comment|Specify the comment for the alert.|True|String||



#### Ping
Test connectivity to the FortiAnalyzer with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Search Logs
Search logs in FortiAnalyzer. Note: Action is running as async, adjust the script timeout value in Siemplify IDE for action as needed.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Log Type|Specify the log type that needs to be searched.|False|List|Traffic|
|Case Sensitive Filter|If enabled, the filter is case sensitive.|False|Boolean|false|
|Query Filter|Specify the query filter for the search.|False|String||
|Device ID|Specify the ID of the device that needs to be searched. If nothing is provided, the action searches in All_Fortigate. Examples of values: All_FortiGate, All_FortiMail, All_FortiWeb, All_FortiManager, All_Syslog, All_FortiClient, All_FortiCache, All_FortiProxy, All_FortiAnalyzer, All_FortiSandbox, All_FortiAuthenticator, All_FortiDDoS.|False|String|All_Fortigate|
|Time Frame|Specify a time frame for the results. If "Custom" is selected, you also need to provide the "Start Time" parameter.|False|List|Last Month|
|Start Time|Specify the start time for the results. This parameter is mandatory, if "Custom" is selected for the "Time Frame" parameter. Format: ISO 8601|False|String||
|End Time|Specify the end time for the results. Format: ISO 8601. If nothing is provided and "Custom" is selected for the "Time Frame" parameter then this parameter uses current time.|False|String||
|Time Order|Specify the time ordering in the search.|False|List|DESC|
|Max Logs To Return|Specify the number of logs you want to return. Default: 20. Maximum: 1000.|False|String|20|



#### Update Alert
Update an alert in FortiAnalyzer.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Alert ID|Specify the ID of the alert that needs to be updated.|True|String||
|Acknowledge Status|Specify the acknowledgment status for alert.|False|List|Select One|
|Mark As Read|If enabled, the action marks the alert as read.|False|Boolean|false|
|Assign To|Specify to whom the alert needs to be assigned.|False|String||



#### Enrich Entities
Enrich entities using information from FortiAnalyzer. Supported entities: Hostname, IP Address.
Timeout - 600 Seconds









## Connectors
#### FortiAnalyzer - Alerts Connector
Pull information about alerts from FortiAnalyzer. Note: Dynamic list filter works with the "subject" parameter.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field through regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|API Root|API root of the FortiAnalyzer instance.|True|String|https://{ip address}|
|Username|Username of the FortiAnalyzer account.|True|String||
|Password|Password of the FortiAnalyzer account.|True|Password|*****|
|Verify SSL|If enabled, verifies that the SSL certificate for the connection to the FortiAnalyzer server is valid.|False|Boolean|true|
|Lowest Severity To Fetch|The lowest severity that needs to be used to fetch alerts. Possible values: low, medium, high, critical. If nothing is specified, the connector ingests alerts with all severities.|False|String|Medium|
|Max Hours Backwards|Number of hours before the first connector iteration to retrieve alerts from. This parameter applies to the initial connector iteration after you enable the connector for the first time, or used as a fallback value in cases where connector's last run timestamp expires.|False|Int|1|
|Max Alerts To Fetch|Number of alerts to process per one connector iteration. Default: 20.|False|Int|20|
|Use dynamic list as a blacklist|If enabled, the dynamic list is used as a blacklist.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




