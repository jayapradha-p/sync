# Microsoft Defender for Endpoint Starting Playbook - 10
Microsoft Defender for Endpoint Starting Playbook provides reference implementation of how Microsoft Defender for Endpoint alerts can be processed in Google SecOps.



**Enabled:** False

**Version:** 0

**Type:** Playbook

**Priority:** 3

**Playbook Simulator:** False


### Playbook Trigger
**Trigger Type:** Custom Trigger

**Conditions Operator:** Or

##### Conditions
|Key|Operator|Value|
|---|--------|-----|
|[Event.event_metadata_logType]|Equals|MICROSOFT_DEFENDER_ENDPOINT|
|[Event.event_metadata_logType]|Equals|MICROSOFT_DEFENDER_ENDPOINT_IOS|
|[Event.event_metadata_logType]|Equals|WINDOWS_DEFENDER_ATP
|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|EDR Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|SUMMARY_DATA init|Action sets a value for a key specified that is stored in the Siemplify database. Available scopes to get context values for: Alert, Case, Global. Action is not working on Siemplify entities. Note: Key Name parameter is case insensitive.|Siemplify|Set Scope Context Value|
|SUMMARY_DATA 1|Action sets a value for a key specified that is stored in the Siemplify database. Available scopes to get context values for: Alert, Case, Global. Action is not working on Siemplify entities. Note: Key Name parameter is case insensitive.|Siemplify|Set Scope Context Value|
|Microsoft Defender for Endpoint Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Set Initial Summary|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Rule Name Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Change Case Name|The action changes the case's name (title)|Tools|Change Case Name|
|Change Stage to Assesment|Change case stage to handling|Siemplify|Change Case Stage|
|Close Alert|Closes the current alert|Siemplify|Close Alert|
|Alert Overview|Fetch information about a detection in Google Chronicle.|GoogleChronicle|Get Detection Details|

### Involved Blocks
|Name|Description|
|----|-----------|
|Google Workspace Enrichment|This block enriches user entities with relevant information from Google Workspace, providing additional context to support investigation and response activities.|
|Microsoft Defender For Endpoint Containment| This block allows the playbook to create an isolate machine task in Microsoft Defender for Endpoint, helping to contain affected systems and prevent further network communication.|
|GTI Enrichment|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|Set Initial Severity|This block sets the initial alert score based on the SIEM detection severity or the rule metadata severity label.|
|MITRE Enrichment|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|Alert Priority|This block sets the alert priority using a previously defined playbook variable, ensuring consistent prioritization logic for the case workflow.|
|High Risk Users Check|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|Google SecOps Enrichment|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Microsoft Defender For Endpoint Enrichment|This block enriches Microsoft Defender for Endpoint hosts by retrieving relevant data such as logged-on users, file-related alerts, and machine-related alerts. It also supports file enrichment using SHA1 hashes, providing additional context to assist investigation and response activities.|
