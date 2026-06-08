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
|Crowdstrike - Incidents Connector|Deprecated. Pull incident and related behaviors from Crowdstrike. Dynamic List works with the “incident_type” parameter.|True|
|Google Chronicle - Chronicle Alerts Connector|Pull information about Rule based alerts from Google Chronicle. Note: dynamic list is used for filtering purposes. For all of the details please visit the documentation portal.|False|


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

