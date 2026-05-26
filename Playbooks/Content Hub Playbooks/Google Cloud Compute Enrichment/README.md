# Google Cloud Compute Enrichment
This block provides additional context about GCP Compute resources related to the case, helping the playbook gain relevant information for analysis and response actions.



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
|Get Instance IAM Policy|Gets the access control policy for the resource. Note that policy may be empty if no policy is assigned to the resource.|GoogleCloudCompute|Get Instance IAM Policy|
|Enrich Entities|Enrich Siemplify IP entities with instance information from Google Cloud Compute.|GoogleCloudCompute|Enrich Entities|

