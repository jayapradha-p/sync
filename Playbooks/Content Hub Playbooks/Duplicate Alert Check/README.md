# Duplicate Alert Check
Is this Alert the first in the Case?  Is it the first in the Case of this Alert type?  Or is it a duplication.  Example usage: this Block can be used when Alert Grouping is causing multiple ITSM tickets for the same case. Different paths output string that can be used in the parent playbook to check the verdict.



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
|Set OtherAlertsExist|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Get OtherAlertsExist|Check if this Block has already run in the Case.|Tools|Get Context Value|
|Set RuleGenerator|Store the Alert type in the Case Context for other Block runs to find.|Tools|Set Context Value|
|FirstOfThisType|Consider building out logic here to update the existing ITSM ticket, e,g, "Add comment: Additional Alerts observed of new type"|Siemplify|Case Comment|
|Set RuleGenerator2|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|AlertTypeExists|Consider building out logic here to update the existing ITSM ticket, e,g, "Add comment: Additional similar Alerts observed"|Siemplify|Case Comment|
|Get RuleGenerator|Check if this RuleGenerator value has been seen in the case.|Tools|Get Context Value|
|FirstOverall|This is the first Alert in the Case, perform all steps as normal. |Siemplify|Case Comment|

