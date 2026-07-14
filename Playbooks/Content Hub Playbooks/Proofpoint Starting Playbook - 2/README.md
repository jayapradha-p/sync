# Proofpoint Starting Playbook - 2
Proofpoint Starting Playbook provides reference implementation of how Proofpoint alerts can be processed in Google SecOps.



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
|[Event.event_metadata_logType]|Contains|PROOFPOINT_MAIL|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|Change Stage to Assesment|Change case stage to handling|Siemplify|Change Case Stage|
|Alert Overview|Fetch information about a detection in Google Chronicle.|GoogleChronicle|Get Detection Details|
|Proofpoint|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Rule Name Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Change Case Name|The action changes the case's name (title)|Tools|Change Case Name|
|Close Alert|Closes the current alert|Siemplify|Close Alert|

### Involved Blocks
|Name|Description|
|----|-----------|
|Set Initial Severity|This block sets the initial alert score based on the SIEM detection severity or the rule metadata severity label.|
|Google Workspace Enrichment|This block enriches user entities with relevant information from Google Workspace, providing additional context to support investigation and response activities.|
|Google SecOps Enrichment|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|GTI Enrichment|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|High Risk Users Check|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|Alert Priority|This block sets the alert priority using a previously defined playbook variable, ensuring consistent prioritization logic for the case workflow.|
|Proofpoint Campaign Details|This block uses the List Campaigns action to retrieve a list of active campaigns in Proofpoint TAP, providing relevant information to support investigation and threat analysis activities.|
|MITRE Enrichment|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
