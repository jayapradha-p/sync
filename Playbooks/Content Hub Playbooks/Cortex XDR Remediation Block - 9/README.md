# Cortex XDR Remediation Block - 9
This block allows the playbook to isolate an endpoint through Cortex XDR, helping to contain potential threats and prevent further compromise.



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
|Isolate Endpoint|Isolate an endpoint.|PaloAltoCortexXDR|Isolate Endpoint|
|Init Remediation|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Hostnames Count|Count the number of entities from a specific scope.|SiemplifyUtilities|Count Entities In Scope|
|IPs Count|Count the number of entities from a specific scope.|SiemplifyUtilities|Count Entities In Scope|
|REMEDIATION_ISOLATE|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|REMEDIATION_NOT_ENDPOINTS|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|REMEDIATION_NOT_ISOLATE|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|

