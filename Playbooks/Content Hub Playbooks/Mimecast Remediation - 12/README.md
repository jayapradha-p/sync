# Mimecast Remediation - 12
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
|Init Remediation|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Create Block Sender Policy|Create a Block Sender policy in Mimecast.|Mimecast|Create Block Sender Policy|
|REMEDIATION 2|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|REMEDIATION 3|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|

