## Sync Alerts
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|https://api.crowdstrike.com|
|Client ID|String|False|ssdsdasd|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|true|
|Client Secret|Password|False|*****|

## Sync Incidents
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** 60

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|True|Default Environment|
|Api Root|String|False||
|Api Key ID|String|True|54|
|Max Hours Backwards|Integer|True|24|
|User Mapping JSON|String|False|{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean|False|false|
|Api Key|Password|True|*****|

