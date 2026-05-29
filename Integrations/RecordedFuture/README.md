
# RecordedFuture

Recorded Future's unique technology collects and analyzes vast amounts of data to deliver relevant cyber threat insights in real-time

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|ApiUrl||True|String|https://api.recordedfuture.com|
|ApiKey||True|Password|*****|
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
#### Enrich CVE
Query the RecordedFuture to get more information about the CVE.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Risk Score Threshold|Represents the minimum malicious risk score for a CVE to be marked malicious. Has a range of 0-99. Has the following levels:  Very Critical: 90-99  Critical: 80-89  High: 65-79  Medium: 25-64  Low: 5-24  None: 0|True|String|25|
|Include Related Entities|If enabled, action will get information about related entities.|False|Boolean|false|



#### Enrich Hash
Query the RecordedFuture to get more information about the hash.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Risk Score Threshold|Represents the minimum malicious risk score for a Hash to be marked malicious. Has a range of 0-89. Has the bands levels:  No Suspicious/Malicious content: 0  Unusual: 5-24  Suspicious: 25-64  Malicious: 65-89|True|String|25|
|Include Related Entities|If enabled, action will get information about related entities.|False|Boolean|false|



#### Enrich IOC
Fetch information about multiple entities, with different types, from Siemplify. Note - we recommend using this action first, and then, if additional information is needed - use the other enrich methods.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Risk Score Threshold|Represents the minimum malicious risk score for each entity to be marked is suspicious.|True|String|25|



#### Get Alert Details
Fetch information about specific Alert and return results to the case. Use action to get more information available regarding Recorded Future Alerts - Documents, Related Entities, Evidence, etc...
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Alert ID|Specify the ID of the alert for which you would like to fetch details|True|String||



#### Get CVE Related Entities
Query the RecordedFuture to get related entities for the CVE.
Timeout - 600 Seconds



#### Get Ip Related Entities
Query the RecordedFuture to get related entities for the IP address.
Timeout - 600 Seconds



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Update Alert
Update alert in Recorded Future.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Alert ID|Specify the ID of the alert that needs to be updated.|True|String||
|Assign To|Specify to whom to assign the alert. You can provide id, username, user hash, or email.|False|String||
|Note|Specify a note that should be updated on the alert.|False|String||
|Status|Specify the new status for the alert.|True|List|Select One|



#### Enrich URL
Query the RecordedFuture to get more information about the URL.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Risk Score Threshold|Represents the minimum malicious risk score for a URL to be marked malicious. Has a range of 0-99. Below is the band levels:  Very Malicious: 90-99  Malicious: 65-89  Suspicious: 25-64  Unusual: 5-24  No Malicious content: 0|True|String|25|
|Include Related Entities|If enabled, action will get information about related entities.|False|Boolean|false|



#### Add Analyst Note
Add an analyst note to previously enriched entities in Siemplify, to Recorded Future entities. Action will add the note to the relevant scope entities. Note: If entity will not contain the Recorded Future ID field - this action will perform “Enrich IOC” action on it for better results. You can choose whether to update the entity with the enrichment data or not.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Note Title|Specify the title for the note|True|String|Note Title|
|Note Text|Specify the Text for the note|True|String|Note Text|
|Note Source|Specify the RF ID for note source; the API explorer shows what the RF IDs are accessible to the user whose API token is enabled. For example,  VWKdVr is the RF ID for an analyst note and is only available to user in the same enterprise account in Recorded Future.|True|String||
|Topic|Specify the relevant Note topic from the list, if needed.|False|List|None|
|Enrich Entity?|Specify whether the action should enrich the entity with the “Enrich IOC” output.|False|Boolean|true|



#### Enrich Host
Query the RecordedFuture to get more information about the Host.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Risk Score Threshold|Represents the minimum malicious risk score for a Host to be marked malicious. Has a range of 0-99. Below is the band levels:  Very Malicious: 90-99  Malicious: 65-89  Suspicious: 25-64  Unusual: 5-24  No Malicious content: 0|True|String|25|
|Include Related Entities|If enabled, action will get information about related entities.|False|Boolean|false|



#### Enrich IP
Query the RecordedFuture to get more information about the IP address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Risk Score Threshold|Represents the minimum malicious risk score for an IP to be marked malicious. Has a range of 0-99. Below is the band levels:  Very Malicious: 90-99  Malicious: 65-89  Suspicious: 25-64  Unusual: 5-24  No Malicious content: 0|True|String|25|
|Include Related Entities|If enabled, action will get information about related entities.|False|Boolean|false|



#### Get Hash Related Entities
Query the RecordedFuture to get related entities for the Hash.
Timeout - 600 Seconds



#### Get Host Related Entities
Query the RecordedFuture to get related entities for the Host.
Timeout - 600 Seconds









## Connectors
#### Recorded Future - Security Alerts Connector
Pull security alerts from Recorded Future. 
Whitelist and blacklist work with Recorded Future rule names.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|API URL|API Root of the Recorded Future instance.|True|String|https://api.recordedfuture.com|
|API Key|API Key of the Recorded Future.|True|Password|*****|
|Fetch Max Hours Backwards|Number of hours before the first connector iteration to retrieve events from. This parameter applies to the initial connector iteration after you enable the connector for the first time, or used as a fallback value in cases where connector's last run timestamp expires.|False|Int|1|
|Max Alerts To Fetch|How many alerts to process per one connector iteration.|False|Int|100|
|Severity|Severity will be one from the following values Low, Medium, High, Critical. Will be assigned to Siemplify alerts created from this connector.|True|String|Medium|
|Get Alert's Details|Get alert's full details from Recorded Future. Note: each query "costs" 1 Recorded Future API credit.|False|Boolean|false|
|Use whitelist as a blacklist|If enabled, whitelist will be used as a blacklist.|False|Boolean|false|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Recorded Future server is valid.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




