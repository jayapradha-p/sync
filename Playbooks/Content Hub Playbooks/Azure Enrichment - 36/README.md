# Azure Enrichment - 36
This block enriches Siemplify Host and User entities with relevant information from Azure Active Directory, providing additional context to support investigation and response activities.



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
|Enrich Host|Enrich Siemplify Host entity with information from Azure Active Directory. Action finds a match for a provided Host entity based on the devices displayName field in Azure AD|AzureActiveDirectory|Enrich Host|
|Enrich User|Enrich Siemplify User entity with information from Azure Active Directory. Action expects Siemplify user entity in username@domain format.|AzureActiveDirectory|Enrich User|

