# Okta Enrichment - 19
This block retrieves information about a user from Okta, including all roles assigned to the user and the groups the user is a member of, providing additional context for analysis and response actions.



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
|List User Groups|Get the groups that the user is a member of|Okta|List User Groups|
|User Details|Get information about a user|Okta|Get User|
|List Roles|Lists all roles assigned to a user|Okta|List Roles|

