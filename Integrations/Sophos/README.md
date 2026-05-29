
# Sophos

Secure cloud workloads, data, apps, and access from the latest advanced threats and vulnerabilities.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|String|https://api.central.sophos.com|
|Client ID||True|String||
|Client Secret||True|Password|*****|
|SIEM API Root||False|String||
|API Key||False|Password|*****|
|Base 64 Auth Payload||False|Password|*****|
|Verify SSL||False|Boolean|True|


#### Dependencies
| |
|-|
|certifi-2026.4.22-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|EnvironmentCommon-1.0.1-py2.py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|TIPCommon-1.0.11-py2.py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|idna-3.13-py3-none-any.whl|


## Actions
#### Enrich Entities
Enrich entities using information from Sophos. Supported entities: Hostname, IP Address, File hash.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Create Insights|If enabled, action will create an insight containing all of the retrieved information about the entity.|False|Boolean|true|



#### Add Entities To Blocklist
Add entities to blocklist in Sophos. Supported entities: Filehash. Note: Only SHA-256 hashes are supported.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Comment|Specify the comment explaining why the hash was sent to blocklist.|True|String||



#### Add Entities To Allowlist
Add entities to allowlist in Sophos. Supported entities: Filehash. Note: Only SHA-256 hashes are supported.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Comment|Specify the comment explaining why the hash was sent to allowlist.|True|String||



#### Get Events Log
Retrieve logs related to the endpoints in Sophos. Supported entities: IP Address, Hostname. Note: events are accessible from API only for 24 hours. Requires valid “SIEM API Root”, “API Key” and “Base 64 Auth Payload” provided in the integration configuration.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Timeframe|Specify how many hours backwards events should be retrieved. Note: if the user provides more than 24 hours, action will still use 24.|True|String|12|
|Max Events To Return|Specify how many events to return per entity. Maximum: 1000|False|String|200|



#### Get Services Status
Retrieve information about services on endpoints in Sophos. Supported entities: IP Address, Hostname.
Timeout - 600 Seconds



#### Isolate Endpoint
Isolate endpoints in Sophos. Supported entities: IP Address, Hostname. Note: Action is running as async, please adjust script timeout value in Siemplify IDE for action as needed.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Comment|Specify the comment explaining why the isolation is needed.|True|String||



#### List Alert Actions
Retrieve actions that can be executed on the alert in Sophos.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Alert ID|Specify the ID of the alert for which you want to retrieve details.|True|String||



#### Execute Alert Actions
Initiate action execution on the alert in Sophos. Use action "List Alert Actions" to get a list of available actions for the alert.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Alert ID|Specify the ID of the alert on which you want to execute the action.|True|String||
|Action|Specify an action that should be executed on the alert.|True|List|Acknowledge|
|Message|Specify a message explaining why the action was executed.|False|String||



#### Ping
Test connectivity to the Sophos with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Scan Endpoints
Initiate a scan on endpoints in Sophos. Supported entities: IP Address, Hostname.
Timeout - 600 Seconds



#### Unisolate Endpoint
Unisolate endpoints in Sophos. Supported entities: IP Address, Hostname. Note: Action is running as async, please adjust script timeout value in Siemplify IDE for action as needed.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Comment|Specify the comment explaining why the unisolation is needed.|True|String||









## Connectors
#### Sophos Central - Alerts Connector
Pull alerts from Sophos Central into Siemplify. Note: alerts are available to API only for 24 hours.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|API Root|API root of the Sophos instance.|True|String|https:/{{api root}}|
|API Key|Sophos API key.|False|Password|*****|
|Base 64 Auth Payload|Sophos Base 64 Auth Payload. Note: "Basic" shouldn't be a part of it.|False|Password|*****|
|Client ID|Sophos Client ID.|False|String||
|Client Secret|Sophos Client Secret.|False|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Sophos Central server is valid.|False|Boolean|true|
|Lowest Severity To Fetch|Severity that will be used to fetch alerts. If nothing is specified, action will ingest all alerts. Possible values: Low, Medium, High.|False|String||
|Max Hours Backwards|Number of hours before the first connector iteration to retrieve alerts from. This parameter applies to the initial connector iteration after you enable the connector for the first time, or used as a fallback value in cases where connector's last run timestamp expires. Maximum is 24 hours.|False|Int|1|
|Max Alerts To Fetch|How many alerts to process per one connector iteration. Maximum is 1000.|False|Int|10|
|Use whitelist as a blacklist|If enabled, whitelist will be used as a blacklist.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




