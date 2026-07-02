# GitSync

## Integrations
|Name|Description|
|----|-----------|
|Google Chronicle|Google SecOps enables you to examine the aggregated security information for your enterprise going back for months or longer. Use Google SecOps to search across all of the domains accessed from within your enterprise. To enable the Google API client to communicate with the Backstory API you will need Google Developer Service Account Credential, https://developers.google.com/identity/protocols/OAuth2#serviceaccount.|
|Google SecOps AI Agents|This integration provides first-party AI agents for Google Chronicle. It allows users to leverage Google's advanced AI capabilities for security operations and threat intelligence within the Chronicle platform.|
|Microsoft Azure Sentinel|Microsoft Azure Sentinel is a scalable, cloud-native, security information event management (SIEM) and security orchestration automated response (SOAR) solution. Azure Sentinel delivers intelligent security analytics and threat intelligence across the enterprise, providing a single solution for alert detection, threat visibility, proactive hunting, and threat response.|
|Microsoft Graph Mail|Microsoft 365 and Office 365 deliver the power of cloud productivity to businesses of all sizes, helping save time, money, and free up valued resources. The Microsoft 365 and Office 365 plans combine the familiar Microsoft Office desktop suite with cloud-based versions of Microsoft's next-generation communications and collaboration services (including Office for the web, Microsoft Exchange Online, Microsoft Teams, and Microsoft SharePoint Online) to help users be productive from virtually anywhere through the Internet. This integration uses Microsoft Graph Mail API to communicate with Microsoft 365 and Office 365 services.|
|Microsoft Graph Security|Microsoft Graph Security provide integrating with Intelligent Security Graph providers that enable your app to retrieve alerts and update alert lifecycle properties|


## Connectors
|Name|Description|Has Mappings|
|----|-----------|------------|
|Anomali Staxx - Indicators Connector|Pull indicators from Anomali Staxx|False|


## Playbooks
|Name|Description|
|----|-----------|
|AWS EC2 Containment|This block allows the playbook to automatically stop EC2 instances that were identified in the alert as potentially compromised or suspicious, supporting the containment phase of the incident response process.|
|AWS Enrichment|This block retrieves EC2 instance data associated with the case and provides context for other actions or analysis.|
|AWS Instance Containment|This block allows you to stop EC2 instances that were identified in the alert as potentially compromised or suspicious, supporting the containment phase of the incident response process.It uses a boolean input to control manual or automatic execution and returns the containment result, false on failure, or an empty value if no action is taken.|
|AWS Users Containment|An embedded workflow that can receive inputs and return an output.|
|Amazon Web Services Cloud Platform Starting Playbook|Amazon Web Services Cloud Platform Starting Playbook provides reference implementation of how Amazon Web Services Cloud Platform alerts can be processed in Google SecOps.|
|Censys - Entity Enrichment|This playbook automatically enriches IP addresses, domains, and certificate entities with Censys threat intelligence data during alert triage and investigation workflows. It retrieves comprehensive asset information including exposed services, ports, protocols, geolocation, ASN details, and associated infrastructure to provide immediate context for security analysts.|
|GTI Enrichment|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|Google SecOps Enrichment|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|MITRE Enrichment|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|New Playbook||
|New Playbook - 1||
|New Block|An embedded workflow that can receive inputs and return an output.|


## Visual Families
|Name|Description|
|----|-----------|
|Test1|testing|


## Jobs
|Name|Description|
|----|-----------|
|hello|This job will sync new SOAR alerts with Chronicle SIEM.Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.|

