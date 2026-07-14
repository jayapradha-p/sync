# Sentinel One Enrichment - 15
This block retrieves information about endpoints from SentinelOne, including details by IP address or hostname, available applications on the endpoint, and associated hashes, providing additional context to support analysis and response activities.



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
|SentinelOne Get Application List For Endpoint|Retrieve information about available applications on the endpoint by IP or Hostname.|SentinelOneV2|Get Application List For Endpoint|
|SentinelOne Enrich Endpoint|Enrich information about the endpoint by IP address or Hostname.|SentinelOneV2|Enrich Endpoint|
|SentinelOne Get Hash Reputation|Retrieve information about the hashes from SentinelOne.|SentinelOneV2|Get Hash Reputation|

