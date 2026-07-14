# Palo Alto Cortex XDR Starting Playbook
Palo Alto Cortex XDR Starting Playbook provides reference implementation of how Palo Alto Cortex XDR alerts can be processed in Google SecOps.



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
|[Event.event_metadata_logType]|Contains|CORTEX_XDR|
|[Event.event_metadata_logType]|Equals|PAN_CORTEX_XDR_EVENTS|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|Reset REMEDIATION Variable|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Close Alert|Closes the current alert|Siemplify|Close Alert|
|Palo Alto Cortex XDR|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Rule Name Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Summary |The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|EDR Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Alert Overview|Fetch information about a detection in Google Chronicle.|GoogleChronicle|Get Detection Details|
|Change Case Name|The action changes the case's name (title)|Tools|Change Case Name|
|PaloAltoCortexXDR Enrich Entities|Enrich Siemplify Host and IP entities based on the information from the Palo Alto Cortex XDR.|PaloAltoCortexXDR|Enrich Entities|
|Set Initial Summary|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Change Stage to Assesment|Change case stage to handling|Siemplify|Change Case Stage|

### Involved Blocks
|Name|Description|
|----|-----------|
|GTI Enrichment|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|Google SecOps Enrichment|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|High Risk Users Check|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|Google Workspace Enrichment|This block enriches user entities with relevant information from Google Workspace, providing additional context to support investigation and response activities.|
|Cortex XDR Remediation Block|This block allows the playbook to isolate an endpoint through Cortex XDR, helping to contain potential threats and prevent further compromise.|
|Alert Priority|This block sets the alert priority using a previously defined playbook variable, ensuring consistent prioritization logic for the case workflow.|
|MITRE Enrichment|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|Set Initial Severity|This block sets the initial alert score based on the SIEM detection severity or the rule metadata severity label.|
