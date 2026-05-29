
# NozomiNetworks

Nozomi Networks Guardianâ„¢ unlocks visibility across OT, IoT, and IT for accelerated security and digital transformation. Its physical or virtual appliances monitor network communications and device behavior, delivering instant awareness of your OT/IoT network and its activity patterns. You see the highest priority vulnerabilities as well as threats and anomalous behavior, enabling you to respond faster, ensuring high reliability and security.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API URL||True|String|https://x.x.x.x:port|
|Username||True|String||
|Password||True|Password|*****|
|Verify SSL||False|Boolean|False|
|CA Certificate File||False|String||


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
#### List Vulnerabilities
List vulnerabilities discovered by Nozomi device based on the provided action input parameters.  Note: Action is not working with Siemplify entities, only with action input parameters.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|IP Address|List vulnerabilities for the provided ip address. Parameter accepts multiple values as a comma separated string.|False|String||
|CVE Score|Minimum CVE score vulnerability should have to be listed, score can be a number from 0 to 10.|False|String||
|Vulnerability Name Contains|Specify a string that vulnerability name should contain to be listed.|False|String||
|CVE ID|If you know specific CVE to look for, provide the related id in this field, for example, CVE-2020-1207. Parameter accepts multiple values as a comma separated string.|False|String||
|Record Limit|Can be used to specify how many records can be returned by the action.|True|String|25|
|Include vulnerabilities that marked as resolved?|Specify whether action should also return vulnerabilities that are marked as resolved.|False|Boolean|false|



#### Run a CLI Command
Run a CLI command on Nozomi Networks device. Note: Nozomi API doesnt provide a validation for executed CLI commands, its up to the User to make sure that the provided CLI command is correct. Note2: Action is not working with Siemplify Entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|CLI Command|Specify a CLI Command to execute on Nozomi Networks device.  Note: Nozomi API doesnt provide a validation for executed CLI commands, its up to the User to make sure that the provided CLI command is correct.|True|String||



#### Run a Query
Run a query on Nozomi Networks device. Note: Action is not working with Siemplify Entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Query|Specify a query to execute on Nozomi Networks device, for example: alerts | head 10|True|String||
|Record Limit|Can be used to specify how many records can be returned by the action. If default value of 10 is set, parameter adds “| head 10” to the final query to limit the number of returned records. If nothing is provided for the parameter - all query results are returned. Negative values are ignored.|False|String|10|



#### Enrich Entities
Enrich Siemplify Host or IP entities based on the information from the Nozomi Networks device.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Additional fields to add to enrichment|Comma separated list of fields that should be additionally taken from Nodes query to add to fields that are used for enrichment by default.|False|String||



#### Ping
Test connectivity to the Nozomi Networks instance with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds









## Connectors
#### Nozomi Networks Alerts Connector
Connector to fetch Nozomi Networks Alerts to Siemplify.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|API URL|Nozomi API URL to connect to.|True|String|https://x.x.x.x:port|
|Username|Nozomi account username to use for connection.|True|String||
|Password|Nozomi account password to use for connection.|True|Password|*****|
|Verify SSL|Specify whether API URL certificate should be validated before connection.|False|Boolean|false|
|CA Certificate File|CA Certificate File - parsed into Base64 String.|False|String||
|Minimum severity to fetch|Minimum severity alert should have to be ingested, severity can be a number from 0 to 10.|False|Int||
|Ingest only alerts that have “is_security” attribute set to True?|Specify if only alerts that have “is_security” attribute set to True should be ingested.|False|Boolean|false|
|Ingest only alerts that have “is_incident” attribute set to True?|Specify if only alerts that have “is_incident” attribute set to True should be ingested.|False|Boolean|false|
|Fetch Max Hours Backwards|Number of hours before the first connector iteration to retrieve alerts from. This parameter applies to the initial connector iteration after you enable the connector for the first time, or used as a fallback value in cases where connector's last run timestamp expires.|True|Int|8|
|Fetch Backwards Time Interval (minutes)|Time interval connector should use to fetch alerts from max hours backwards. If Nozomi Device is deployed in a large network, the number of generated alerts can be substantial. Because of this, this parameter in minutes can be used to split max hours backwards on smaller segments and process them individually. Time interval cant be bigger than max hours backwards value.|True|Int|60|
|Use whitelist as a blacklist|If enabled, whitelist will be used as a blacklist.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




