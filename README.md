# GitSync

## Integrations
|Name|Description|
|----|-----------|
|new integration|None|


## Connectors
|Name|Description|Has Mappings|
|----|-----------|------------|
|Palo Alto Cortex XDR Connector|Pull incidents from Palo Alto XDR. Dynamic List works with the “source” parameter.|True|


## Playbooks
|Name|Description|
|----|-----------|
|Azure AD Enrichment|This block enriches Siemplify Host and User entities with relevant information from Azure Active Directory, providing additional context to support investigation and response activities.|
|Clean Case|Clean case (Tags, Alert scoring info, etc) when playbooks that are often rerun and can create duplicate evidence.  Extend this logic to meet your requirements.|
|Copy of Copy of New Playbook - 9||
|Copy of Copy of New Playbook - 9 - 10||
|Copy of Copy of New Playbook - 9 - 11||
|Copy of Copy of New Playbook - 9 - 12||
|Copy of Copy of New Playbook - 9 - 13||
|Copy of Copy of New Playbook - 9 - 14||
|Copy of Copy of New Playbook - 9 - 15||
|Copy of Copy of New Playbook - 9 - 16||
|Copy of Copy of New Playbook - 9 - 17||
|Copy of Copy of New Playbook - 9 - 2||
|Copy of Copy of New Playbook - 9 - 3||
|Copy of Copy of New Playbook - 9 - 4||
|Copy of Copy of New Playbook - 9 - 5||
|Copy of Copy of New Playbook - 9 - 6||
|Copy of Copy of New Playbook - 9 - 7||
|Copy of Copy of New Playbook - 9 - 8||
|Copy of Copy of New Playbook - 9 - 9||
|Copy of New Playbook||
|Copy of New Playbook - 1||
|Copy of New Playbook - 1 - 2||
|Copy of New Playbook - 1 - 3||
|Copy of New Playbook - 10||
|Copy of New Playbook - 11||
|Copy of New Playbook - 12||
|Copy of New Playbook - 13||
|Copy of New Playbook - 14||
|Copy of New Playbook - 15||
|Copy of New Playbook - 16||
|Copy of New Playbook - 17||
|Copy of New Playbook - 18||
|Copy of New Playbook - 19||
|Copy of New Playbook - 2||
|Copy of New Playbook - 20||
|Copy of New Playbook - 21||
|Copy of New Playbook - 22||
|Copy of New Playbook - 23||
|Copy of New Playbook - 24||
|Copy of New Playbook - 25||
|Copy of New Playbook - 26||
|Copy of New Playbook - 27||
|Copy of New Playbook - 28||
|Copy of New Playbook - 29||
|Copy of New Playbook - 3||
|Copy of New Playbook - 30||
|Copy of New Playbook - 31||
|Copy of New Playbook - 32||
|Copy of New Playbook - 4||
|Copy of New Playbook - 5||
|Copy of New Playbook - 6||
|Copy of New Playbook - 7||
|Copy of New Playbook - 8||
|Copy of New Playbook - 9||
|New Block|An embedded workflow that can receive inputs and return an output.|
|New Playbook||


## Jobs
|Name|Description|
|----|-----------|
|Sync Incidents|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|

