# SentinelOne Starting Playbook - 2
SentinelOne Starting Playbook provides reference implementation of how SentinelOne alerts can be processed in Google SecOps.



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
|[Event.event_metadata_logType]|Equals|SENTINELONE_ACTIVITY
|
|[Event.event_metadata_logType]|Equals|SENTINEL_EDR|
|[Event.event_metadata_logType]|Equals|SENTINEL_DV|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|Rule Name Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Alert Overview|Fetch information about a detection in Google Chronicle.|GoogleChronicle|Get Detection Details|
|SUMMARY_DATA 1|Action sets a value for a key specified that is stored in the Siemplify database. Available scopes to get context values for: Alert, Case, Global. Action is not working on Siemplify entities. Note: Key Name parameter is case insensitive.|Siemplify|Set Scope Context Value|
|Sentinel One Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Set Initial Summary|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|EDR Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Change Stage to Assesment|Change case stage to handling|Siemplify|Change Case Stage|
|Close Alert|Closes the current alert|Siemplify|Close Alert|
|SUMMARY_DATA reset|Action sets a value for a key specified that is stored in the Siemplify database. Available scopes to get context values for: Alert, Case, Global. Action is not working on Siemplify entities. Note: Key Name parameter is case insensitive.|Siemplify|Set Scope Context Value|
|Change Case Name|The action changes the case's name (title)|Tools|Change Case Name|

### Involved Blocks
|Name|Description|
|----|-----------|
|High Risk Users Check|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|Sentinel One Enrichment|This block retrieves information about endpoints from SentinelOne, including details by IP address or hostname, available applications on the endpoint, and associated hashes, providing additional context to support analysis and response activities.|
|GTI Enrichment|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|Alert Priority|This block sets the alert priority using a previously defined playbook variable, ensuring consistent prioritization logic for the case workflow.|
|Google SecOps Enrichment|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Set Initial Severity|This block sets the initial alert score based on the SIEM detection severity or the rule metadata severity label.|
|Sentinel One Containment|This block filters the relevant entities and performs containment actions in SentinelOne, including adding hashes to a blacklist and disconnecting the endpoint agent from the network using its hostname or IP address.|
