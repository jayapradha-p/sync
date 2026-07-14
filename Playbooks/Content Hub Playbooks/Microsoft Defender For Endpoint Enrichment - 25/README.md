# Microsoft Defender For Endpoint Enrichment - 25
This block enriches Microsoft Defender for Endpoint hosts by retrieving relevant data such as logged-on users, file-related alerts, and machine-related alerts. It also supports file enrichment using SHA1 hashes, providing additional context to assist investigation and response activities.



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
|MicrosoftDefender Related Alerts|Get Machine Related Alerts|MicrosoftDefenderATP|Get Machine Related Alerts|
|Machine Logon Users|Get Machine Log on users|MicrosoftDefenderATP|Get Machine Logon Users|
|MicrosoftDefender File Related Alerts|Get File Related Alerts. Note: For this action only SHA1 is supported|MicrosoftDefenderATP|Get File Related Alerts|
|Microsoft Defender Enrich Entities|This action allows a user to enrich Microsoft Defender ATP hosts, ips and file hashes. Note: File hash can be in sha1 or sha256 format.|MicrosoftDefenderATP|Enrich Entities|

