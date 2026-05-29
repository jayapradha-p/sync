
# RSANetWitnessPlatform

RSA NetWitness Platform accelerates threat detection and response by collecting and analyzing data across more capture points (logs, packets, netflow and endpoint) and computing platforms (physical, virtual and cloud) and enriching this data with threat intelligence and business context.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Broker API Root||False|IP_OR_HOST|http://x.x.x.x:50103|
|Broker API Username||False|String||
|Broker API Password||False|Password|*****|
|Concentrator API Root||False|IP_OR_HOST|http://x.x.x.x:50105|
|Concentrator API Username||False|String||
|Concentrator API Password||False|Password|*****|
|Web API Root||False|IP_OR_HOST|https://{ip}/rest/api/|
|Web Username||False|String||
|Web Password||False|Password|*****|
|Verify SSL||False|Boolean|True|


#### Dependencies
| |
|-|
|certifi-2026.4.22-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|EnvironmentCommon-1.0.1-py2.py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|TIPCommon-1.0.12-py2.py3-none-any.whl|
|idna-3.13-py3-none-any.whl|


## Actions
#### Enrich File
Fetch information about the file using hashes or file names. Only MD5 and SHA256 are supported. Requires RSA Netwitness Respond license, endpoint server service running in the background, configured Web Username and Web Password in the integration configuration.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Risk Score Threshold|Specify risk threshold for the file. If the file exceeds the threshold, the related entity will be marked as suspicious. If nothing is specified, action won’t check the risk score.|False|String|50|



#### Update Incident
Update Incident in RSA Netwitness. Requires RSA Netwitness Respond license, configured Web Username and Web Password in the integration configuration.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Incident ID|Specify ID of the incident that needs to be updated.|True|String||
|Status|Specify new status for the incident.|False|List||
|Assignee|Specify new assignee for the incident.|False|String||



#### Run General Query
Run free query and receive event and a PCAP file.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Query|Custom query string.|True|String|None|
|Max Hours Backwards|Specify how many hours backwards to fetch events. Default is 1 hour.|False|String|1|
|Max Events To Return|Specify how many events to return. If nothing is specified, action will return 50 events.|False|String|50|



#### Query NetWitness For Events Around Host
Retrieve the latest events related to the hostnames in RSA Netwitness. Requires configuration of Broker API or Concentrator API
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Max Hours Backwards|Specify how many hours backwards to fetch events. Default is 1 hour.|False|String|1|
|Max Events To Return|Specify how many events to return. If nothing is specified, action will return 50 events.|False|String|50|



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Enrich Endpoint
Fetch endpoint's system information by its hostname or IP address. Requires RSA Netwitness Respond license, endpoint server service running in the background, configured Web Username and Web Password in the integration configuration.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Risk Score Threshold|Specify risk threshold for the endpoint. If the endpoint exceeds the threshold, the related entity will be marked as suspicious. If nothing is specified, action won’t check the risk score.|False|String|50|



#### Isolate Endpoint
Request endpoint isolation in RSA Netwitness. Requires RSA Netwitness Respond license, endpoint server service running in the background, configured Web Username and Web Password in the integration configuration.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Comment|Add comment, which describes the reason behind the isolation request.|True|String||



#### Unisolate Endpoint
Request endpoint unisolation in RSA Netwitness. Requires RSA Netwitness Respond license, endpoint server service running in the background, configured Web Username and Web Password in the integration configuration.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Comment|Add comment, which describes the reason behind the unisolation request.|True|String||



#### Add Note to Incident
Add Note to Incident in RSA Netwitness. Requires RSA Netwitness Respond license, configured Web Username and Web Password in the integration configuration.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Incident ID|Specify ID of the incident that needs to be updated.|True|String||
|Note|Specify which note should be added to.|True|String||
|Author|Specify the author of the note.|True|String||



#### Query NetWitness For Events Around User
Run a query on RSA NetWitness to retreive all events for a specific query (conditions) for a given username in the alert
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Max Hours Backwards|Specify how many hours backwards to fetch events. Default is 1 hour.|False|String|1|
|Max Events To Return|Specify how many events to return. If nothing is specified, action will return 50 events.|False|String|50|



#### Query NetWitness For Events Around IP
Run a query on RSA NetWitness to retreive all events for a specific query (conditions) for a given IP address in the alert
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Max Hours Backwards|Specify how many hours backwards to fetch events. Default is 1 hour.|False|String|1|
|Max Events To Return|Specify how many events to return. If nothing is specified, action will return 50 events.|False|String|50|









## Connectors
#### RSA Netwitness Platform - Incidents Connector
Pull incidents from RSA Netwitness Platform.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Disable Overflow|If enabled, connector will ignore the overflow mechanism.|False|Boolean|true|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|Web API Root|Web API Root of the RSA Netwitness Platform instance.|True|String|https://{ip}/rest/api|
|Web Username|Username of the RSA Netwitness Platform account.|True|String||
|Web Password|Password of the RSA Netwitness Platform account.|True|Password|*****|
|Broker API Root|API Root of the RSA Netwitness broker. Note: broker configuration takes priority over concentrator. Example: https://{ip}:50103. If this parameter is provided, the connector will try to fetch more context related to the incident.|False|String||
|Broker API Username|API Username of the RSA Netwitness broker. Note: broker configuration takes priority over concentrator. If this parameter is provided, the connector will try to fetch more context related to the incident.|False|String||
|Broker API Password|API Password of the RSA Netwitness broker. Note: broker configuration takes priority over concentrator. If this parameter is provided, the connector will try to fetch more context related to the incident.|False|Password|*****|
|Concentrator API Root|API Root of the RSA Netwitness concentrator. Note: broker configuration takes priority over concentrator. Example: https://{ip}:50105. If this parameter is provided, the connector will try to fetch more context related to the incident.|False|String||
|Concentrator API Username|API Username of the RSA Netwitness concentrator. Note: broker configuration takes priority over concentrator. If this parameter is provided, the connector will try to fetch more context related to the incident.|False|String||
|Concentrator API Password|API Password of the RSA Netwitness concentrator. Note: broker configuration takes priority over concentrator. If this parameter is provided, the connector will try to fetch more context related to the incident.|False|Password|*****|
|Credential JSON Object|This parameter is needed for storing the data source credentials. This parameter has priority over "Broker API Root", "Broker API Username", "Broker API Password", "Concentrator API Root", "Concentrator API Username", "Concentrator API Password". Please refer to the documentation portal for more details.|False|Password|*****|
|Fetch Max Hours Backwards|Number of hours before the first connector iteration to retrieve incidents from. This parameter applies to the initial connector iteration after you enable the connector for the first time, or used as a fallback value in cases where connector's last run timestamp expires. Note: connector will wait for the provided time for the updates to incidents.|False|Int|1|
|Lowest Risk Score To Fetch|Lowest risk score of the incidents to fetch. By default, the connector will ingest all of the incidents. Maximum is 100.|False|Int||
|Severity Fallback|Specify what should be the fallback severity for the Siemplify Alert, when risk score is not available. Possible values: Informational, Low, Medium, High, Critical.|True|String|Informational|
|Max Incidents To Fetch|How many incidents to process per one connector iteration. Maximum is 100.|False|Int|10|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the RSA Netwitness Plaform server is valid.|False|Boolean|false|
|Use whitelist as a blacklist|If enabled, whitelist will be used as a blacklist.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




