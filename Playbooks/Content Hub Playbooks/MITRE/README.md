# MITRE
This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and potential defensive actions. It receives an Add Tag boolean input; when set to true, it adds the MITRE technique ID to the case.



**Enabled:** True

**Version:** 0

**Type:** Block

**Priority:** 2

**Playbook Simulator:** False


##### Input Parameters
|Name|Default Value|
|----|-------------|
|Add Tag|True|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|Add Technique Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Mitre Techniques Mitigations|Retrieve information about mitigations that are associated with MITRE attack techniques.|MitreAttck|Get Techniques Mitigations|
|Mitre Techniques Details|Retrieve detailed information about MITRE attack techniques.|MitreAttck|Get Techniques Details|

