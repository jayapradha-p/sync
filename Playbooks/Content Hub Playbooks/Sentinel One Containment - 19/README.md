# Sentinel One Containment - 19
This block filters the relevant entities and performs containment actions in SentinelOne, including adding hashes to a blacklist and disconnecting the endpoint agent from the network using its hostname or IP address.



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
|REMEDIATION 1|Action sets a value for a key specified that is stored in the Siemplify database. Available scopes to get context values for: Alert, Case, Global. Action is not working on Siemplify entities. Note: Key Name parameter is case insensitive.|Siemplify|Set Scope Context Value|
|REMEDIATION 2|Action sets a value for a key specified that is stored in the Siemplify database. Available scopes to get context values for: Alert, Case, Global. Action is not working on Siemplify entities. Note: Key Name parameter is case insensitive.|Siemplify|Set Scope Context Value|
|SentinelOne Create Hash Blacklist Record|Add hashes to a blacklist in SentinelOne. Note: Only SHA1 hashes are supported.|SentinelOneV2|Create Hash Blacklist Record|
|Count File hashes|Count the number of entities from a specific scope.|SiemplifyUtilities|Count Entities In Scope|
|Init Remediation|Action sets a value for a key specified that is stored in the Siemplify database. Available scopes to get context values for: Alert, Case, Global. Action is not working on Siemplify entities. Note: Key Name parameter is case insensitive.|Siemplify|Set Scope Context Value|
|Isolate Endpoint|Disconnect agent from network by it's host name or IP address.|SentinelOneV2|Disconnect Agent From Network|
|Remediation 4|Action sets a value for a key specified that is stored in the Siemplify database. Available scopes to get context values for: Alert, Case, Global. Action is not working on Siemplify entities. Note: Key Name parameter is case insensitive.|Siemplify|Set Scope Context Value|
|Remediation 3|Action sets a value for a key specified that is stored in the Siemplify database. Available scopes to get context values for: Alert, Case, Global. Action is not working on Siemplify entities. Note: Key Name parameter is case insensitive.|Siemplify|Set Scope Context Value|

