
# HarmonyMobile

Harmony Mobile is the market-leading Mobile Threat Defense solution. It keeps your corporate data safe by securing employees’ mobile devices across all attack vectors: apps, network and OS. Designed to reduce admins’ overhead and increase user adoption, it perfectly fits into your existing mobile environment, deploys and scales quickly, and protects devices without impacting user experience nor privacy.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|String|https://cloudinfra-gw.portal.checkpoint.com|
|Client ID||True|String||
|Client Secret||True|Password|*****|
|Verify SSL||False|Boolean|true|


#### Dependencies
| |
|-|
|certifi-2026.4.22-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|EnvironmentCommon-1.0.0-py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|idna-3.13-py3-none-any.whl|


## Actions
#### Enrich Entities
Enrich entities using information from Harmony Mobile. Supported entities: Hostname. Note: Hostname entity should contain the "name" of the device.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Create Insight|If enabled, action will create an insight containing all of the retrieved information about the entity.|False|Boolean|true|



##### JSON Results
```json
[{"Entity": "test", "EntityResult": {"client_version": "3.8.x.xxxx", "device_type": "Android", "email": "test@example.com", "internal_id": "1x", "last_connection": "Fri, 30 Jul 2021 08:27:11 +0000", "mail_sent": true, "mdm": null, "model": "HUAWEI / HUAWEI GRA-L09", "name": "test", "number": "+11", "os_type": "Android_4_x", "os_version": "6.0", "risk": "High", "status": "Active"}}, {"Entity": "Trial Device", "EntityResult": {"client_version": "3.8.x.xxxx", "device_type": "Android", "email": "trial@test.com", "internal_id": "2x", "last_connection": "Sun, 18 Jul 2021 13:07:59 +0000", "mdm": null, "model": "HUAWEI / HMA-L29", "name": "Trial Device", "number": "123456789", "os_type": "Android_4_x", "os_version": "10", "risk": "Medium", "status": "Active"}}]
```



#### Ping
Test connectivity to the Harmony Mobile with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds









## Connectors
#### Harmony Mobile - Alerts Connector
Pull information about alerts from Harmony Mobile. Note: whitelist filter works with "threat_factors" parameter.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|DeviceProductField|Enter the source field name in order to retrieve the Product Field name.|True|String|Product Name|
|EventClassId|Enter the source field name in order to retrieve the Event Field name.|True|String|alertType|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|PythonProcessTimeout|Timeout limit for the python process running the current script.|True|Integer|180|
|API Root|API root of the Harmony Mobile instance.|True|String|https://cloudinfra-gw.portal.checkpoint.com|
|Client ID|Client ID of the Harmony Mobile account.|True|String||
|Client Secret|Client Secret of the Harmony Mobile account. |True|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Harmony Mobile server is valid.|False|Boolean|true|
|Lowest Risk To Fetch|Lowest risk that needs to be used to fetch alerts. Possible values: Informational, Low, Medium, High. If nothing is specified, the connector will ingest alerts with all risk levels.|False|String||
|Max Hours Backwards|Number of hours before the first connector iteration to retrieve alerts from. This parameter applies to the initial connector iteration after you enable the connector for the first time, or used as a fallback value in cases where connector's last run timestamp expires.|False|Integer|1|
|Max Alerts To Fetch|How many alerts to process per one connector iteration. Default: 100.|False|Integer|100|
|Use whitelist as a blacklist|If enabled, whitelist will be used as a blacklist.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




