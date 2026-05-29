
# SiemplifyThreatFuse

ThreatFuse combines best-in-class security orchestration, automation and response (SOAR) with a market-leading Threat Intelligence Platform (TIP) powered by Anomali, to make intelligence-driven security operations simple and accessible for organizations of all sizes.With robust integration out of the box, ThreatFuse ingrains threat-intelligence across the entire detection and response lifecycle. From enrichment with real-time threat indicators, through threat-hunting and intelligence sharing, security analysts can validate, investigate and respond to threats with unprecedented speed and precision.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Web Root|None|True|String|https://siemplify.threatstream.com|
|API Root|None|True|String|https://api.threatstream.com|
|Email Address|None|True|String||
|API Key|None|True|Password|*****|
|Verify SSL|None|False|Boolean||


#### Dependencies
| |
|-|
|tzdata-2024.1-py2.py3-none-any.whl|
|numpy-2.1.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|
|chardet-5.2.0-py3-none-any.whl|
|pytz-2024.1-py2.py3-none-any.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|six-1.16.0-py2.py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|idna-3.8-py3-none-any.whl|
|EnvironmentCommon-1.0.0-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|
|python_dateutil-2.9.0.post0-py2.py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|
|pandas-2.2.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|
|certifi-2024.8.30-py3-none-any.whl|


## Actions
#### Enrich Entities
Retrieve information about IPs, URLs, hashes or User entities with Email regexes from Siemplify ThreatFuse. If multiple records are found for the same entity, action will enrich using the latest record.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Severity Threshold|Specify what should be the severity threshold for the entity, in order to mark it as suspicious. If multiple records are found for the same entity, action will take the highest severity out of all available records.|True|List|Low|
|Confidence Threshold|Specify what should be the confidence threshold for the entity, in order to mark it as suspicious. Note: Maximum is 100. If multiple records are found for the entity, action will take the average. Active records have priority.|True|String||
|Ignore False Positive Status|If enabled, action will ignore the false positive status and mark the entity as suspicious based on the "Severity Threshold" and "Confidence Threshold". If disabled, action will never label false positive entities as suspicious, regardless, if they pass the "Severity Threshold" and "Confidence Threshold" conditions or not.|False|Boolean|false|
|Add Threat Type To Case|If enabled, action will add threat types of the entity from all records as tags to the case. Example: apt|False|Boolean|false|
|Create Insight|If enabled, action will add an insight per processed entity.|False|Boolean|false|
|Only Suspicious Entity Insight|If enabled, action will create insight only for entities that exceeded the "Severity Threshold" and "Confidence Threshold".|False|Boolean|false|



#### Get Related Associations
Retrieve entity related associations from Siemplify ThreatFuse. Configure the parameters below: choose the association types to return, specify Max Associations To Return. You can also choose to add retrieved associations as entities to the case.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Return Campaigns|If enabled, action will fetch related campaigns and details about them.|False|Boolean|True|
|Return Threat Bulletins|If enabled, action will fetch related threat bulletins and details about them.|False|Boolean|False|
|Return Actors|If enabled, action will fetch related actors and details about them.|False|Boolean|False|
|Return Attack Patterns|If enabled, action will fetch related attack patterns and details about them.|False|Boolean|False|
|Return Courses Of Action|If enabled, action will fetch related courses of action and details about them.|False|Boolean|False|
|Return Identities|If enabled, action will fetch related identities and details about them.|False|Boolean|False|
|Return Incidents|If enabled, action will fetch related incidents and details about them.|False|Boolean|False|
|Return Infrastructure|If enabled, action will fetch related infrastructure and details about them.|False|Boolean|False|
|Return Intrusion Sets|If enabled, action will fetch related intrusion sets and details about them.|False|Boolean|False|
|Return Malware|If enabled, action will fetch related malware and details about them.|False|Boolean|False|
|Return Signatures|If enabled, action will fetch related signatures and details about them.|False|Boolean|False|
|Return Tools|If enabled, action will fetch related tools and details about them.|False|Boolean|False|
|Return TTPs|If enabled, action will fetch related TTPs and details about them.|False|Boolean|False|
|Return Vulnerabilities|If enabled, action will fetch related vulnerabilities and details about them.|False|Boolean|True|
|Create Campaign Entity|If enabled, action will create an entity out of available “Campaign” associations.|False|Boolean|False|
|Create Actors Entity|If enabled, action will create an entity out of available “Actor” associations.|False|Boolean|False|
|Create Signature Entity|If enabled, action will create an entity out of available “Signature” associations.|False|Boolean|False|
|Create Vulnerability Entity|If enabled, action will create an entity out of available “Vulnerability” associations.|False|Boolean|False|
|Create Case Tag|If enabled, action will create case tags based on the results.|False|Boolean|True|
|Create Insight|If enabled, action will create an insight base on the results.|False|Boolean|True|
|Max Associations To Return|Specify how many associations to return per type. Default: 5|False|String|5|
|Max Statistics To Return|Specify how many top statistics results regarding IOCs to return. Note: action will at max process 1000 IOCs related to the association. If you provide "0", action will not try to fetch statistics information.|False|String|3|



#### Ping
Test connectivity to the Siemplify ThreatFuse with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Submit Observables
Submit an observable to Siemplify ThreatFuse based on IP, URL, Hash or User entities with Email regexes from Siemplify ThreatFuse. Note: requires 'Org admin', 'Create Anomali Community Intel' and 'Approve Intel' permissions.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Classification|Specify the classification of the observable.|True|List|Private|
|Threat Type|Specify the threat type of the observables.|True|List|APT|
|Source|Specify the intelligence source for the observable.|False|String|Siemplify|
|Expiration Date|Specify the expiration date in days for the observable. If nothing is specified here, action will create an observable that will never expire.|False|String||
|Trusted Circle IDs|Specify the comma-separated list of trusted circle ids. Observables will be shared with those trusted circles.|False|String||
|TLP|Specify the TLP for your observables.|False|List|Select One|
|Confidence|Specify what should be the confidence for the observable. Note: this parameter will only work, if you create observables in your organization and requires 'Override System Confidence' to be enabled.|False|String||
|Override System Confidence|If enabled, created observables will have the confidence specified in the 'Confidence' parameter. Note: you can't share observables in trusted circles and publicly, when this parameter is enabled.|False|Boolean|False|
|Anonymous Submission|If enabled, action will make an anonymous submission.|False|Boolean|False|
|Tags|Specify a comma-separated list of tags that you want to add to observable.|False|String||



#### Get Related IPs
Retrieve entity related IP addresses based on the associations in Siemplify ThreatFuse. Supported entities: Hash, URL, IP Address, Email Address (user entity that matches email regex), Threat Actor, CVE.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Confidence Threshold|Specify what should be the confidence threshold. Note: Maximum is 100.|True|String||
|Search Observables|If enabled, action will search among observables.|False|Boolean|True|
|Search Threat Bulletins|If enabled, action will search among threat bulletins.|False|Boolean|True|
|Search Actors|If enabled, action will search among actors.|False|Boolean|True|
|Search Attack Patterns|If enabled, action will search among attack patterns.|False|Boolean|True|
|Search Campaigns|If enabled, action will search among campaigns.|False|Boolean|True|
|Search Courses Of Action|If enabled, action will search among courses of action.|False|Boolean|True|
|Search Identities|If enabled, action will search among identities.|False|Boolean|True|
|Search Incidents|If enabled, action will search among incidents.|False|Boolean|True|
|Search Infrastructures|If enabled, action will search among infrastructures.|False|Boolean|True|
|Search Intrusion Sets|If enabled, action will search among intrusion sets.|False|Boolean|True|
|Search Malware|If enabled, action will search among malware.|False|Boolean|True|
|Search Signatures|If enabled, action will search among signatures.|False|Boolean|True|
|Search Tools|If enabled, action will search among tools.|False|Boolean|True|
|Search TTPs|If enabled, action will search among TTPs.|False|Boolean|True|
|Search Vulnerabilities|If enabled, action will search among vulnerabilities.|False|Boolean|True|
|Max IPs To Return|Specify how many IPs to return. Default: 50.|False|String|50|



#### Get Related URLs
Retrieve entity related urls based on the associations in Siemplify ThreatFuse. Supported entities: Hash, URL, IP Address, Email Address (user entity that matches email regex), Threat Actor, CVE.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Confidence Threshold|Specify what should be the confidence threshold. Note: Maximum is 100.|True|String||
|Search Threat Bulletins|If enabled, action will search among threat bulletins.|False|Boolean|True|
|Search Actors|If enabled, action will search among actors.|False|Boolean|True|
|Search Attack Patterns|If enabled, action will search among attack patterns.|False|Boolean|True|
|Search Campaigns|If enabled, action will search among campaigns.|False|Boolean|True|
|Search Courses Of Action|If enabled, action will search among courses of action.|False|Boolean|True|
|Search Identities|If enabled, action will search among identities.|False|Boolean|True|
|Search Incidents|If enabled, action will search among incidents.|False|Boolean|True|
|Search Infrastructures|If enabled, action will search among infrastructures.|False|Boolean|True|
|Search Intrusion Sets|If enabled, action will search among intrusion sets.|False|Boolean|True|
|Search Malware|If enabled, action will search among malware.|False|Boolean|True|
|Search Signatures|If enabled, action will search among signatures.|False|Boolean|True|
|Search Tools|If enabled, action will search among tools.|False|Boolean|True|
|Search TTPs|If enabled, action will search among TTPs.|False|Boolean|True|
|Search Vulnerabilities|If enabled, action will search among vulnerabilities.|False|Boolean|True|
|Max URLs To Return|Specify how many hashes to return. Default: 50.|False|String|50|



#### Get Related Domains
Retrieve entity related domains based on the associations in Siemplify ThreatFuse. Supported entities: Hash, URL, IP Address, Email Address (user entity that matches email regex), Threat Actor, CVE.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Confidence Threshold|Specify what should be the confidence threshold. Note: Maximum is 100.|True|String||
|Search Threat Bulletins|If enabled, action will search among threat bulletins.|False|Boolean|True|
|Search Actors|If enabled, action will search among actors.|False|Boolean|True|
|Search Attack Patterns|If enabled, action will search among attack patterns.|False|Boolean|True|
|Search Campaigns|If enabled, action will search among campaigns.|False|Boolean|True|
|Search Courses Of Action|If enabled, action will search among courses of action.|False|Boolean|True|
|Search Identities|If enabled, action will search among identities.|False|Boolean|True|
|Search Incidents|If enabled, action will search among incidents.|False|Boolean|True|
|Search Infrastructures|If enabled, action will search among infrastructures.|False|Boolean|True|
|Search Intrusion Sets|If enabled, action will search among intrusion sets.|False|Boolean|True|
|Search Malware|If enabled, action will search among malware.|False|Boolean|True|
|Search Signatures|If enabled, action will search among signatures.|False|Boolean|True|
|Search Tools|If enabled, action will search among tools.|False|Boolean|True|
|Search TTPs|If enabled, action will search among TTPs.|False|Boolean|True|
|Search Vulnerabilities|If enabled, action will search among vulnerabilities.|False|Boolean|True|
|Max Domains To Return|Specify how many domains to return. Default: 50.|False|String|50|



#### Get Related Hashes
Retrieve entity related hashes based on the associations in Siemplify ThreatFuse. Supported entities: Hash, URL, IP Address, Email Address (user entity that matches email regex), Threat Actor, CVE.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Confidence Threshold|Specify what should be the confidence threshold. Note: Maximum is 100.|True|String||
|Search Threat Bulletins|If enabled, action will search among threat bulletins.|False|Boolean|True|
|Search Actors|If enabled, action will search among actors.|False|Boolean|True|
|Search Attack Patterns|If enabled, action will search among attack patterns.|False|Boolean|True|
|Search Campaigns|If enabled, action will search among campaigns.|False|Boolean|True|
|Search Courses Of Action|If enabled, action will search among courses of action.|False|Boolean|True|
|Search Identities|If enabled, action will search among identities.|False|Boolean|True|
|Search Incidents|If enabled, action will search among incidents.|False|Boolean|True|
|Search Infrastructures|If enabled, action will search among infrastructures.|False|Boolean|True|
|Search Intrusion Sets|If enabled, action will search among intrusion sets.|False|Boolean|True|
|Search Malware|If enabled, action will search among malware.|False|Boolean|True|
|Search Signatures|If enabled, action will search among signatures.|False|Boolean|True|
|Search Tools|If enabled, action will search among tools.|False|Boolean|True|
|Search TTPs|If enabled, action will search among TTPs.|False|Boolean|True|
|Search Vulnerabilities|If enabled, action will search among vulnerabilities.|False|Boolean|True|
|Max Hashes To Return|Specify how many hashes to return. Default: 50.|False|String|50|



#### Get Related Email Addresses
Retrieve entity related email addresses based on the associations in Siemplify ThreatFuse. Supported entities: Hash, URL, IP Address, Email Address (user entity that matches email regex), Threat Actor, CVE.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Confidence Threshold|Specify what should be the confidence threshold. Note: Maximum is 100.|True|String||
|Search Observables|If enabled, action will search among observables.|False|Boolean|True|
|Search Threat Bulletins|If enabled, action will search among threat bulletins.|False|Boolean|True|
|Search Actors|If enabled, action will search among actors.|False|Boolean|True|
|Search Attack Patterns|If enabled, action will search among attack patterns.|False|Boolean|True|
|Search Campaigns|If enabled, action will search among campaigns.|False|Boolean|True|
|Search Courses Of Action|If enabled, action will search among courses of action.|False|Boolean|True|
|Search Identities|If enabled, action will search among identities.|False|Boolean|True|
|Search Incidents|If enabled, action will search among incidents.|False|Boolean|True|
|Search Infrastructures|If enabled, action will search among infrastructures.|False|Boolean|True|
|Search Intrusion Sets|If enabled, action will search among intrusion sets.|False|Boolean|True|
|Search Malware|If enabled, action will search among malware.|False|Boolean|True|
|Search Signatures|If enabled, action will search among signatures.|False|Boolean|True|
|Search Tools|If enabled, action will search among tools.|False|Boolean|True|
|Search TTPs|If enabled, action will search among TTPs.|False|Boolean|True|
|Search Vulnerabilities|If enabled, action will search among vulnerabilities.|False|Boolean|True|
|Max Email Addresses To Return|Specify how many email addresses to return. Default: 50.|False|String|50|









## Connectors
#### Siemplify ThreatFuse - Observables Connector
Pull observables from Siemplify ThreatFuse. Note: Source names are used in the whitelist.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|API root of the Siemplify ThreatFuse instance.|True|String|https://api.threatstream.com|
|Email Address|Email address of the Siemplify ThreatFuse account.|True|String||
|API Key|API Key of the Siemplify ThreatFuse account.|True|Password|*****|
|Lowest Severity To Fetch|Lowest severity that will be used to fetch observables. Possible values: Low, Medium, High, Very-High|True|String|High|
|Lowest Confidence To Fetch|Lowest confidence that will be used to fetch observables. Maximum is 100.|True|Int|50|
|Source Feed Filter|Comma-separated list of feed ids that should be used to ingest observables. Example: 515,4129|False|String||
|Observable Type Filter|Comma-separated list of observable types that should be  ingested. Example: url, domain. Possible values: url, domain, email, hash, ip, ipv6|False|String|url, domain, email, hash, ip, ipv6|
|Observable Status Filter|Comma-separated list of observable status that should be used to ingest new data. Example: active, inactive. Possible values: active, inactive, falsepos|False|String|active|
|Threat Type Filter|Comma-separated list of threat types that should be used to ingest observables. Example: аdware, anomalous, anonymization, apt. Possible values: аdware, anomalous, anonymization, apt,bot,brute, c2,compromised, crypto,data_leakage, ddos, dyn_dns, exfil, exploit, fraud, hack_tool, i2p, informational, malware, p2p, parked, phish, scan, sinkhole, spam, suppress, suspicious, tor, vps|False|String||
|Trusted Circle Filter|Comma-separated list of trusted circle ids that should be used to ingest observables. Example: 146,147|False|String||
|Tag Name Filter|Comma-separated list of tag names associated with observables that should be used with ingestion. Example: Microsoft Credentials, Phishing|False|String||
|Source Feed Grouping|If enabled, the connector will group observables from the same source under the same Siemplify Alert.|False|Boolean|false|
|Fetch Max Days Backwards|Number of days before the first connector iteration to retrieve findings from. This parameter applies to the initial connector iteration after you enable the connector for the first time, or used as a fallback value in cases where connector's last run timestamp expires.|False|Int|1|
|Max Observables Per Alert|How many observables should be a part of one Siemplify Alert. Maximum is 200.|False|Int|100|
|Use whitelist as a blacklist|If enabled, whitelist will be used as a blacklist.|False|Boolean|false|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Siemplify ThreatFuse server is valid.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




