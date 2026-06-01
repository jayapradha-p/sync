## projects/project/locations/location/instances/instance/integrations/PaloAltoCortexXDR/jobs/787/jobInstances/68
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
||String|False|Default Environment|
||String|False||
||String|False|54|
||Int|False|24|
||String|False|{"Google SecOps Display Name": "XDR Username"}|
||Boolean|False|false|
||Password|False|*****|

