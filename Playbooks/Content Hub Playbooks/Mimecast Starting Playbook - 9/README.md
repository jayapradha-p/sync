# Mimecast Starting Playbook - 9
Mimecast Starting Playbook provides reference implementation of how Mimecast alerts can be processed in Google SecOps.




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
|[Event.event_metadata_logType]|Contains|MIMECAST_MAIL|
|[Event.entity_metadata_vendorName]|Equals|Mimecast|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|Set Initial Summary|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Close Alert|Closes the current alert|Siemplify|Close Alert|
|Change Stage to Assesment|Change case stage to handling|Siemplify|Change Case Stage|
|Rule Name Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Change Case Name|The action changes the case's name (title)|Tools|Change Case Name|
|Alert Overview|Fetch information about a detection in Google Chronicle.|GoogleChronicle|Get Detection Details|
|Summary |The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Mimecast|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Reset REMEDIATION Variable|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|

### Involved Blocks
|Name|Description|
|----|-----------|
|Alert Priority|This block sets the alert priority using a previously defined playbook variable, ensuring consistent prioritization logic for the case workflow.|
|Set Initial Severity|This block sets the initial alert score based on the SIEM detection severity or the rule metadata severity label.|
|Google Workspace Enrichment|This block enriches user entities with relevant information from Google Workspace, providing additional context to support investigation and response activities.|
|MITRE Enrichment|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|High Risk Users Check|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|GTI Enrichment|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|Google SecOps Enrichment|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Mimecast Investigation|This block performs an investigation by searching archived emails in Mimecast based on specified parameters and returns relevant information to support analysis and response activities within the case.|
|Mimecast Remediation|This block allows the playbook to create a Block Sender policy in Mimecast to prevent future emails from a specified sender, or to take no action if required.|
