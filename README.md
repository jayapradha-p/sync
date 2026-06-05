# GitSync

## Integrations
|Name|Description|
|----|-----------|
|CrowdStrike Falcon|CrowdStrike Falcon is the leader in next-generation endpoint protection, threat intelligence and incident response through cloud-based endpoint protection.|
|Exchange|Integration provides support for Microsoft Exchange 2010 - 2019 and Microsoft Office365 mail servers. Integration uses Exchange Web Services (EWS) for communication. Integration includes a series of actions to send out emails and work with received emails, along with a connector to monitor specific mailboxes and ingest emails from that mailboxes as alerts to Google SecOps for further analysis.|
|Google Chronicle|Google SecOps enables you to examine the aggregated security information for your enterprise going back for months or longer. Use Google SecOps to search across all of the domains accessed from within your enterprise. To enable the Google API client to communicate with the Backstory API you will need Google Developer Service Account Credential, https://developers.google.com/identity/protocols/OAuth2#serviceaccount.|
|Google SecOps AI Agents|This integration provides first-party AI agents for Google Chronicle. It allows users to leverage Google's advanced AI capabilities for security operations and threat intelligence within the Chronicle platform.|
|Microsoft Azure Sentinel|Microsoft Azure Sentinel is a scalable, cloud-native, security information event management (SIEM) and security orchestration automated response (SOAR) solution. Azure Sentinel delivers intelligent security analytics and threat intelligence across the enterprise, providing a single solution for alert detection, threat visibility, proactive hunting, and threat response.|
|Microsoft Graph Mail|Microsoft 365 and Office 365 deliver the power of cloud productivity to businesses of all sizes, helping save time, money, and free up valued resources. The Microsoft 365 and Office 365 plans combine the familiar Microsoft Office desktop suite with cloud-based versions of Microsoft's next-generation communications and collaboration services (including Office for the web, Microsoft Exchange Online, Microsoft Teams, and Microsoft SharePoint Online) to help users be productive from virtually anywhere through the Internet. This integration uses Microsoft Graph Mail API to communicate with Microsoft 365 and Office 365 services.|
|Microsoft Graph Mail Delegated|This integration version uses Delegated Authentication in Microsoft 365 and requires interactive login of the user on behalf of which integration should communicate with Microsoft 365. To configure this integration, provide all parameters except for Refresh Token, and save the integration configuration, then run “Get Authorization” and “Generate Token” actions to get the token and then provide it in integration configuration to finish the process. Microsoft 365 and Office 365 deliver the power of cloud productivity to businesses of all sizes, helping save time, money, and free up valued resources. The Microsoft 365 and Office 365 plans combine the familiar Microsoft Office desktop suite with cloud-based versions of Microsoft's next-generation communications and collaboration services (including Office for the web, Microsoft Exchange Online, Microsoft Teams, and Microsoft SharePoint Online) to help users be productive from virtually anywhere through the Internet. This integration uses Microsoft Graph Mail API to communicate with Microsoft 365 and Office 365 services.|
|Microsoft Teams|Microsoft Teams is a platform that combines workplace chat, meetings, notes, and attachmentsQuick Guide: you must first register your app at Microsoft App Registration Portal, Configure Microsoft Teams Integration, Run the action 'Get Authorization', Run the action 'Generate Token'.|
|Palo Alto Cortex XDR|Cortex XDR - XDR is the world’s first detection and response app that natively integrates network, endpoint and cloud data to stop sophisticated attacks.  Cortex XDR accurately detects threats with behavioral analytics and reveals the root cause to speed up investigations.|
|SentinelOne|Endpoint security software that defends every endpoint against every type of attack, at every stage in the threat lifecycle.|
|SentinelOneV2|Endpoint security software that defends every endpoint against every type of attack, at every stage in the threat lifecycle.|


## Connectors
|Name|Description|Has Mappings|
|----|-----------|------------|
|Palo Alto Cortex XDR Connector|Pull incidents from Palo Alto XDR. Dynamic List works with the “source” parameter.|False|


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
|projects/project/locations/location/instances/instance/integrations/CaServiceDesk/jobs/1252/jobInstances/117|Sync closure of the tickets at the CA Desk Manager with Siemplify cases closure.|
|projects/project/locations/location/instances/instance/integrations/CaServiceDesk/jobs/1252/jobInstances/86|Sync closure of the tickets at the CA Desk Manager with Siemplify cases closure.|
|projects/project/locations/location/instances/instance/integrations/GoogleChronicle/jobs/786/jobInstances/82|This job will sync new SOAR alerts with Chronicle SIEM.Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.|
|projects/project/locations/location/instances/instance/integrations/GoogleChronicle/jobs/786/jobInstances/116|This job will sync new SOAR alerts with Chronicle SIEM.Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.|
|projects/project/locations/location/instances/instance/integrations/GoogleChronicle/jobs/786/jobInstances/110|This job will sync new SOAR alerts with Chronicle SIEM.Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.|
|projects/project/locations/location/instances/instance/integrations/GoogleChronicle/jobs/785/jobInstances/83|This job will synchronize information about Chronicle SOAR Cases and Chronicle SOAR Alerts with Chronicle SIEM. Note: This job is only supported from Chronicle SOAR version 6.1.44 and higher.|
|projects/project/locations/location/instances/instance/integrations/GoogleChronicle/jobs/785/jobInstances/84|This job will synchronize information about Chronicle SOAR Cases and Chronicle SOAR Alerts with Chronicle SIEM. Note: This job is only supported from Chronicle SOAR version 6.1.44 and higher.|
|projects/project/locations/location/instances/instance/integrations/GoogleChronicle/jobs/785/jobInstances/124|This job will synchronize information about Chronicle SOAR Cases and Chronicle SOAR Alerts with Chronicle SIEM. Note: This job is only supported from Chronicle SOAR version 6.1.44 and higher.|
|projects/project/locations/location/instances/instance/integrations/AzureSecurityCenter/jobs/869/jobInstances/94|Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.|
|projects/project/locations/location/instances/instance/integrations/MicrosoftTeams/jobs/873/jobInstances/103|Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.|
|projects/project/locations/location/instances/instance/integrations/AzureSecurityCenter/jobs/869/jobInstances/112|Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.|
|projects/project/locations/location/instances/instance/integrations/AzureSecurityCenter/jobs/869/jobInstances/88|Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.|
|projects/project/locations/location/instances/instance/integrations/CrowdStrikeFalcon/jobs/1657/jobInstances/79|This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/CrowdStrikeFalcon/jobs/1657/jobInstances/111|This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/CrowdStrikeFalcon/jobs/1657/jobInstances/115|This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/SentinelOneV2/jobs/875/jobInstances/118|This job will synchronize Google SecOps Alerts and SentinelOne alerts. The job synchronizes status. Requires “SentinelOne Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” you will need to add an “Alert_ID” Alert Context Value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/SentinelOneV2/jobs/875/jobInstances/119|This job will synchronize Google SecOps Alerts and SentinelOne alerts. The job synchronizes status. Requires “SentinelOne Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” you will need to add an “Alert_ID” Alert Context Value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/SentinelOneV2/jobs/875/jobInstances/120|This job will synchronize Google SecOps Alerts and SentinelOne alerts. The job synchronizes status. Requires “SentinelOne Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” you will need to add an “Alert_ID” Alert Context Value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/CrowdStrikeFalcon/jobs/1657/jobInstances/125|This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/CrowdStrikeFalcon/jobs/1657/jobInstances/91|This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/SentinelOneV2/jobs/875/jobInstances/97|This job will synchronize Google SecOps Alerts and SentinelOne alerts. The job synchronizes status. Requires “SentinelOne Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” you will need to add an “Alert_ID” Alert Context Value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/CrowdStrikeFalcon/jobs/1657/jobInstances/105|This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/CrowdStrikeFalcon/jobs/1657/jobInstances/108|This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/SentinelOneV2/jobs/875/jobInstances/109|This job will synchronize Google SecOps Alerts and SentinelOne alerts. The job synchronizes status. Requires “SentinelOne Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” you will need to add an “Alert_ID” Alert Context Value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/CrowdStrikeFalcon/jobs/1657/jobInstances/74|This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/CaServiceDesk/jobs/1251/jobInstances/122|Sync comments from CA Desk Manager to Siemplify.|
|projects/project/locations/location/instances/instance/integrations/CaServiceDesk/jobs/1251/jobInstances/78|Sync comments from CA Desk Manager to Siemplify.|
|projects/project/locations/location/instances/instance/integrations/CaServiceDesk/jobs/1251/jobInstances/92|Sync comments from CA Desk Manager to Siemplify.|
|projects/project/locations/location/instances/instance/integrations/CaServiceDesk/jobs/1251/jobInstances/98|Sync comments from CA Desk Manager to Siemplify.|
|projects/project/locations/location/instances/instance/integrations/CaServiceDesk/jobs/1251/jobInstances/99|Sync comments from CA Desk Manager to Siemplify.|
|projects/project/locations/location/instances/instance/integrations/CaServiceDesk/jobs/1251/jobInstances/81|Sync comments from CA Desk Manager to Siemplify.|
|projects/project/locations/location/instances/instance/integrations/CaServiceDesk/jobs/1251/jobInstances/101|Sync comments from CA Desk Manager to Siemplify.|
|projects/project/locations/location/instances/instance/integrations/CaServiceDesk/jobs/1251/jobInstances/76|Sync comments from CA Desk Manager to Siemplify.|
|projects/project/locations/location/instances/instance/integrations/PaloAltoCortexXDR/jobs/1658/jobInstances/113|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/PaloAltoCortexXDR/jobs/1658/jobInstances/114|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/PaloAltoCortexXDR/jobs/1658/jobInstances/77|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/PaloAltoCortexXDR/jobs/1658/jobInstances/95|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/PaloAltoCortexXDR/jobs/1658/jobInstances/126|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/PaloAltoCortexXDR/jobs/1658/jobInstances/90|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/PaloAltoCortexXDR/jobs/1658/jobInstances/96|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/MicrosoftAzureSentinel/jobs/870/jobInstances/123|Use the Sync Incidents V2 job to synchronize Google SecOps alerts with Microsoft Sentinel incidents. This job ensures that comments, statuses, and tags are synchronized bi-directionally between both systems. Note: Assignee and severity synchronization occurs exclusively from Microsoft Sentinel to Google SecOps. For the job to identify the correct information, the Google SecOps case must have the Microsoft Sentinel Incident tag. This job only works on alerts from the Microsoft Azure Sentinel Incident Connector v2.|
|projects/project/locations/location/instances/instance/integrations/PaloAltoCortexXDR/jobs/1658/jobInstances/75|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/SentinelOneV2/jobs/874/jobInstances/121|This job will synchronize Google SecOps Alerts and SentinelOne threats. The job synchronizes comments and status. Requires “SentinelOne Threat” tag on the case. Note: If the alert didn’t originate from “Threats Connector” you will need to add an “Threat_ID” Alert Context Value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/SentinelOneV2/jobs/874/jobInstances/104|This job will synchronize Google SecOps Alerts and SentinelOne threats. The job synchronizes comments and status. Requires “SentinelOne Threat” tag on the case. Note: If the alert didn’t originate from “Threats Connector” you will need to add an “Threat_ID” Alert Context Value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/SentinelOneV2/jobs/874/jobInstances/107|This job will synchronize Google SecOps Alerts and SentinelOne threats. The job synchronizes comments and status. Requires “SentinelOne Threat” tag on the case. Note: If the alert didn’t originate from “Threats Connector” you will need to add an “Threat_ID” Alert Context Value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/SentinelOneV2/jobs/874/jobInstances/87|This job will synchronize Google SecOps Alerts and SentinelOne threats. The job synchronizes comments and status. Requires “SentinelOne Threat” tag on the case. Note: If the alert didn’t originate from “Threats Connector” you will need to add an “Threat_ID” Alert Context Value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/Exchange/jobs/1301/jobInstances/85|Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.|
|projects/project/locations/location/instances/instance/integrations/Exchange/jobs/1301/jobInstances/100|Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.|
|projects/project/locations/location/instances/instance/integrations/Exchange/jobs/1301/jobInstances/80|Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.|

