# GitSync

## Connectors
|Name|Description|Has Mappings|
|----|-----------|------------|
|ArcSight - Security Events Connector|Pull correlations from ArcSight. Note: dynamic list works with "name" parameter. Please refer to the doc portal for the configuration setup. This connector is suitable for Saas deployment of Chronicle SOAR and is the recommended one for production use.|False|
|Palo Alto Cortex XDR Connector|Pull incidents from Palo Alto XDR. Dynamic List works with the “source” parameter.|False|
|VirusTotal - Livehunt Notifications Connector|Pull information about Livehunt notifications and related files from VirusTotal. Note: this connector requires a premium API token. Dynamic list works with "rule_name" parameter.|False|


## Playbooks
|Name|Description|
|----|-----------|
|New Playbook||
|New Playbook - 2||
|New Playbook - new folder||
|New Playbook - new2||


## Visual Families
|Name|Description|
|----|-----------|
|Test1|Testing|
|Test2|Testing|


## Jobs
|Name|Description|
|----|-----------|
|projects/project/locations/location/instances/instance/integrations/GoogleChronicle/jobs/2/jobInstances/4|This job will sync new SOAR alerts with Chronicle SIEM.Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.|
|projects/project/locations/location/instances/instance/integrations/PaloAltoCortexXDR/jobs/42/jobInstances/3|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|

