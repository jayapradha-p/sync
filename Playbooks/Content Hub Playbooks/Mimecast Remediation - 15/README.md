# Mimecast Remediation - 15
This block allows the playbook to create a Block Sender policy in Mimecast to prevent future emails from a specified sender, or to take no action if required.



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
|Create Block Sender Policy|Create a Block Sender policy in Mimecast.|Mimecast|Create Block Sender Policy|
|REMEDIATION 3|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Init Remediation|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|REMEDIATION 2|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|

