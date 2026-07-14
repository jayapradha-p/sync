# Symantec Enrichment and Investigation - 7
This block supports remediation by retrieving system information for endpoints and listing all endpoints/sensors and groups configured on a specified Symantec-managed device, providing the necessary context for follow-up actions.



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
|Get System Info|Get system information for endpoints|SEP|GetSystemInfo|
|List Groups|List all the groups configured on a particular device|SEP|ListGroups|
|List Endpoints| List all the endpoints/sensors configured on a particular device|SEP|ListEndpoints|

