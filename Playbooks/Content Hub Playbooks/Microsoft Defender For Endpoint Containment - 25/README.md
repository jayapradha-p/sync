# Microsoft Defender For Endpoint Containment - 25
 This block allows the playbook to create an isolate machine task in Microsoft Defender for Endpoint, helping to contain affected systems and prevent further network communication.



**Enabled:** True

**Version:** 0

**Type:** Block

**Priority:** 2

**Playbook Simulator:** False


##### Input Parameters
|Name|Default Value|
|----|-------------|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|Init Remediation|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|COMPUTE_INSTANCE_REMEDIATION_SUMMARY |The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Isolate Machine|Create Isolate Machine Task|MicrosoftDefenderATP|Create Isolate Machine Task|
|Count Instances|Count the number of entities from a specific scope.|SiemplifyUtilities|Count Entities In Scope|
|NO_COMPUTE_INSTANCE_REMEDIATION_SUMMARY|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Count Local IPs|Count the number of entities from a specific scope.|SiemplifyUtilities|Count Entities In Scope|

