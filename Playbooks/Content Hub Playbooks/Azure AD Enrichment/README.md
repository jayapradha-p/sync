# Azure AD Enrichment
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
|Enrich User|Enrich Siemplify User entity with information from Azure Active Directory. Action expects Siemplify user entity in username@domain format.|AzureActiveDirectory|Enrich User|
|List User's Groups Membership|List Azure AD groups user is a member of. Note: The user name can be provided either as a Siemplify entity or as an action input parameter. If the user name is passed to action both as an entity and input parameter - action will be executed on the input parameter. User name should be specified in username@domain format.|AzureActiveDirectory|List User's Groups Membership|
|Enrich Host|Enrich Siemplify Host entity with information from Azure Active Directory. Action finds a match for a provided Host entity based on the devices displayName field in Azure AD|AzureActiveDirectory|Enrich Host|
|Get Manager Contact Details|Get manager contact details for user. Action expects Siemplify user entity in username@domain format.|AzureActiveDirectory|Get Manager Contact Details|

