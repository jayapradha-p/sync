## Sync Alerts
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** 60

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Client Secret|Password|True|*****|
|Environment Name|String|True|Default Environment|
|API Root|String|True|https://api.crowdstrike.com|
|Client ID|String|True|ssdsdasd|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|true|

