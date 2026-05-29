# GitSync

## Integrations
|Name|Description|
|----|-----------|
|Abnormal Security|Abnormal Security uses AI to protect organizations from email attacks. This integration enables automated ingestion of threats and cases as SOAR alerts, plus search and remediation of malicious email messages through the Abnormal Security API. For support, contact: support@abnormalsecurity.com|
|AbuseIPDB|Leverage the AbuseIPDB threat intelligence API with this integration.|
|Active Directory|Microsoft Active Directory integration facilitates the centralized management and synchronization of Windows user accounts with Security Center's administrator and cardholder accounts.|
|AirTable|Airtable can store information in a spreadsheet that's visually appealing and easy-to-use, but it's also powerful enough to act as a database that businesses can use for customer-relationship management (CRM), task management, project planning, and tracking inventory.|
|Akamai|Akamai provides security services deployed across a global edge network. This includes Web Application Firewall (WAF) capabilities identifying web-based attacks, Bot Management distinguishing between human and automated traffic, DDoS mitigation services absorbing malicious traffic floods, and API security protections. Akamai generates security event data reflecting threats detected and actions taken at the internet edge.|
|Alexa|The Alexa Web Information Service (AWIS) offers a platform for creating innovative Web solutions and services based on Alexa's vast information about web sites.|


## Connectors
|Name|Description|Has Mappings|
|----|-----------|------------|
|Palo Alto Cortex XDR Connector|Pull incidents from Palo Alto XDR. Dynamic List works with the “source” parameter.|False|


## Playbooks
|Name|Description|
|----|-----------|
|Azure AD Enrichment|This block enriches Siemplify Host and User entities with relevant information from Azure Active Directory, providing additional context to support investigation and response activities.|
|Clean Case|Clean case (Tags, Alert scoring info, etc) when playbooks that are often rerun and can create duplicate evidence.  Extend this logic to meet your requirements.|
|New Block|An embedded workflow that can receive inputs and return an output.|
|New Playbook||


## Jobs
|Name|Description|
|----|-----------|
|projects/project/locations/location/instances/instance/integrations/CrowdStrikeFalcon/jobs/50/jobInstances/27|This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/PaloAltoCortexXDR/jobs/58/jobInstances/28|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|

