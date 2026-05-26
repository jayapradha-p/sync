# Zscaler Containment
This block allows you to add a URL, domain, or IP address to the Zscaler blacklist as part of containment actions, helping prevent further access to potentially harmful resources. It uses a boolean input to control manual or automatic execution and returns the containment result, false on failure, or an empty value if no action is taken.



**Enabled:** True

**Version:** 0

**Type:** Block

**Priority:** 2

**Playbook Simulator:** False


##### Input Parameters
|Name|Default Value|
|----|-------------|
|Manual|True|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|Add To Blacklist Auto|Adds a URL/Domain/IP to black list.|Zscaler|Add To Blacklist|
|Add To Blacklist|Adds a URL/Domain/IP to black list.|Zscaler|Add To Blacklist|

