# BloodHound Attack Path Alerts Playbook
Triages BloodHound Enterprise Attack Path alerts ingested via the Attack Paths Alert connector. Resolves involved entities to BloodHound object IDs, checks whether the attack paths still exist, fetches asset metadata, and routes alerts based on environment context for SOC investigation.



**Enabled:** False

**Version:** 0

**Type:** Playbook

**Priority:** 1

**Playbook Simulator:** False


### Playbook Trigger
**Trigger Type:** All

**Conditions Operator:** And

##### Conditions
|Key|Operator|Value|
|---|--------|-----|
||Equals||


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|BloodHound Enterprise_Does Path Exists_2||BloodHound Enterprise|Does Path Exists|
|Fetch Assets_3||BloodHound Enterprise|Fetch Assets|
|BloodHound Enterprise_Does Path Exists_1||BloodHound Enterprise|Does Path Exists|
|Get Object Id_3||BloodHound Enterprise|Get Object Id|
|BloodHound Enterprise_Get Object Id_2||BloodHound Enterprise|Get Object Id|
|BloodHound Enterprise_Fetch Assets_2||BloodHound Enterprise|Fetch Assets|
|Does Path Exists_3||BloodHound Enterprise|Does Path Exists|
|BloodHound Enterprise_Fetch Assets_1||BloodHound Enterprise|Fetch Assets|
|BloodHound Enterprise_Get Object Id_1||BloodHound Enterprise|Get Object Id|

