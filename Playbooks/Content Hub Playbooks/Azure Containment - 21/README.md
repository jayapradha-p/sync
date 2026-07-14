# Azure Containment - 21
This block allows the playbook to apply containment actions to Azure user accounts by either updating the password or disabling the account. It also provides the option to ignore the action and take no changes when required.



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
|REMEDIATION Force Password Update|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|REMEDIATION Do Nothing|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Disable Account|Disable account in Azure Active Directory. Action expects Siemplify user entity in username@domain format.|AzureActiveDirectory|Disable Account|
|REMEDIATION Disable Account|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Init Remediation|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Force Password Update|Force password update for user so the user will have to change their password on next login. Action expects Siemplify user entity in username@domain format.|AzureActiveDirectory|Force Password Update|

