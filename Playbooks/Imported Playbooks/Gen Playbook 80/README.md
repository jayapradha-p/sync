# Gen Playbook 80
This playbook retrieves and analyzes historical scan data for IP addresses to identify infrastructure changes, service modifications, and temporal patterns. It helps analysts understand how an asset has evolved over time, detect anomalous changes, establish baseline behavior, and correlate infrastructure changes with security events.



**Enabled:** False

**Version:** 0

**Type:** Playbook

**Priority:** 3

**Playbook Simulator:** False


### Playbook Trigger
**Trigger Type:** All

**Conditions Operator:** And

##### Conditions
|Key|Operator|Value|
|---|--------|-----|
||Equals||


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|Get Host History|This action retrieves the event history for a host (IP address). It allows users to view historical scan data, track infrastructure changes over time, and identify when services were added, removed, or modified.|Censys|Get Host History|

