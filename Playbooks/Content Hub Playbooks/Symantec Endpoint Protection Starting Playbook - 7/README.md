# Symantec Endpoint Protection Starting Playbook - 7
Symantec Endpoint Protection Starting Playbook provides reference implementation of how Symantec Endpoint Protection alerts can be processed in Google SecOps.



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
|[Event.event_metadata_logType]|Contains|SYMANTEC_EVENT_EXPORT|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|Change Case Name|The action changes the case's name (title)|Tools|Change Case Name|
|Insert Black List Name|The Spell Check String action will check the spelling of an input string.  It will output the percent accurate, total words, amount of misspelled words, list of each misspelled word and the correction, and a corrected version of the input string.|Tools|Spell Check String|
|Set Initial Summary|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Close Alert|Closes the current alert|Siemplify|Close Alert|
|Rule Name Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Black List Name|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Summary |The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|SYMANTEC_BLACK_LIST_NAME|The action gets a key and value in a specific context (alert or case)|Tools|Get Context Value|
|Reset REMEDIATION Variable|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Add Symantec Endpoint Protection Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Alert Overview|Fetch information about a detection in Google Chronicle.|GoogleChronicle|Get Detection Details|
|Change Stage to Assesment|Change case stage to handling|Siemplify|Change Case Stage|

### Involved Blocks
|Name|Description|
|----|-----------|
|Alert Priority|This block sets the alert priority using a previously defined playbook variable, ensuring consistent prioritization logic for the case workflow.|
|Set Initial Severity|This block sets the initial alert score based on the SIEM detection severity or the rule metadata severity label.|
|Google Workspace Enrichment|This block enriches user entities with relevant information from Google Workspace, providing additional context to support investigation and response activities.|
|Google SecOps Enrichment|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Symantec Remediation|This block offers guidance to support remediation activities by suggesting actions such as quarantining suspicious endpoints or blocking malicious hashes, helping analysts take appropriate corrective measures during the response process.|
|Symantec Enrichment and Investigation|This block supports remediation by retrieving system information for endpoints and listing all endpoints/sensors and groups configured on a specified Symantec-managed device, providing the necessary context for follow-up actions.|
|High Risk Users Check|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|MITRE Enrichment|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|GTI Enrichment|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
