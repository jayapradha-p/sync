# Copy of Copy of New Playbook - 9




**Enabled:** True

**Version:** 0

**Type:** Playbook

**Priority:** 2

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
|Siemplify_Assign Case_1|Use the "Assign Case" action to assign the case to a user.|Siemplify|Assign Case|
|GitSync_Ping_1|Test connectivity to GitSync|GitSync|Ping|
|Siemplify_Case Comment_1|Add a comment to the case the current alert has been grouped to|Siemplify|Case Comment|

### Involved Blocks
|Name|Description|
|----|-----------|
|New Block|An embedded workflow that can receive inputs and return an output.|
