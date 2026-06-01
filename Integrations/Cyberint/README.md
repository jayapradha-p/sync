
# Cyberint

Digital Risk Protection that turns intelligence into actions to proactively and effectively defend businesses against cyber threats.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|String|https://{instance}.cyberint.io|
|API Key||True|Password|*****|
|Verify SSL||False|Boolean|true|


#### Dependencies
| |
|-|
|urllib3-2.6.3-py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|certifi-2026.4.22-py3-none-any.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|EnvironmentCommon-1.0.0-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|idna-3.13-py3-none-any.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|


## Actions
#### Update Alert
Update alert in Cyberint.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Alert ID|Specify the id of the alert that would need to have the status updated.|True|String||
|Status|Specify the status for the event. Note: if "Closed" is selected, "Closure Reason" needs to be provided as well.|False|List|Select One|
|Closure Reason|Specify the closure reason for closed status.|False|List|Select One|



#### Ping
Test connectivity to the Cyberint with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds









## Connectors
#### Cyberint - Alerts Connector
Pull information about alerts from Cyberint. Note: whitelist filter works with "alertEvent" parameter.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|DeviceProductField|Enter the source field name in order to retrieve the Product Field name.|True|String|Product Name|
|EventClassId|Enter the source field name in order to retrieve the Event Field name.|True|String|type|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|PythonProcessTimeout|Timeout limit for the python process running the current script.|True|Integer|180|
|API Root|API root of the Cyberint instance.|True|String|https://{instance}.cyberint.io|
|API Key|API key of the Cyberint instance.|True|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Cyberint server is valid.|False|Boolean|true|
|Lowest Severity To Fetch|Lowest risk that needs to be used to fetch alerts. Possible values: Low, Medium, High, Very High. If nothing is specified, the connector will ingest alerts with all severities|False|String||
|Max Hours Backwards|Number of hours before the first connector iteration to retrieve alerts from. This parameter applies only once to the initial connector iteration after you enable the connector for the first time.|False|Integer|1|
|Max Alerts To Fetch|How many alerts to process per one connector iteration. Default: 100.|False|Integer|100|
|Use whitelist as a blacklist|If enabled, whitelist will be used as a blacklist.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




