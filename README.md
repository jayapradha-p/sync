# GitSync

## Integrations
|Name|Description|
|----|-----------|
|Azure Active Directory|Azure Active Directory (Azure AD) is Microsoft's cloud-based identity and access management service, which helps your employees sign in and access  both internal and external resources.|
|CSV|Integration designed around working with CSV files. CSV is a simple file format used to store tabular data, such as a spreadsheet or database.|
|CrowdStrike Falcon|CrowdStrike Falcon is the leader in next-generation endpoint protection, threat intelligence and incident response through cloud-based endpoint protection.|
|EmailUtilities|A set of utility actions to assist with working with emails.  Includes actions to parse EMLs and analyze email headers.|
|Google Chronicle|Google SecOps enables you to examine the aggregated security information for your enterprise going back for months or longer. Use Google SecOps to search across all of the domains accessed from within your enterprise. To enable the Google API client to communicate with the Backstory API you will need Google Developer Service Account Credential, https://developers.google.com/identity/protocols/OAuth2#serviceaccount.|
|Google SecOps AI Agents|This integration provides first-party AI agents for Google Chronicle. It allows users to leverage Google's advanced AI capabilities for security operations and threat intelligence within the Chronicle platform.|
|Microsoft Azure Sentinel|Microsoft Azure Sentinel is a scalable, cloud-native, security information event management (SIEM) and security orchestration automated response (SOAR) solution. Azure Sentinel delivers intelligent security analytics and threat intelligence across the enterprise, providing a single solution for alert detection, threat visibility, proactive hunting, and threat response.|
|Microsoft Graph Mail|Microsoft 365 and Office 365 deliver the power of cloud productivity to businesses of all sizes, helping save time, money, and free up valued resources. The Microsoft 365 and Office 365 plans combine the familiar Microsoft Office desktop suite with cloud-based versions of Microsoft's next-generation communications and collaboration services (including Office for the web, Microsoft Exchange Online, Microsoft Teams, and Microsoft SharePoint Online) to help users be productive from virtually anywhere through the Internet. This integration uses Microsoft Graph Mail API to communicate with Microsoft 365 and Office 365 services.|
|Microsoft Graph Mail Delegated|This integration version uses Delegated Authentication in Microsoft 365 and requires interactive login of the user on behalf of which integration should communicate with Microsoft 365. To configure this integration, provide all parameters except for Refresh Token, and save the integration configuration, then run “Get Authorization” and “Generate Token” actions to get the token and then provide it in integration configuration to finish the process. Microsoft 365 and Office 365 deliver the power of cloud productivity to businesses of all sizes, helping save time, money, and free up valued resources. The Microsoft 365 and Office 365 plans combine the familiar Microsoft Office desktop suite with cloud-based versions of Microsoft's next-generation communications and collaboration services (including Office for the web, Microsoft Exchange Online, Microsoft Teams, and Microsoft SharePoint Online) to help users be productive from virtually anywhere through the Internet. This integration uses Microsoft Graph Mail API to communicate with Microsoft 365 and Office 365 services.|
|Microsoft Graph Security|Microsoft Graph Security provide integrating with Intelligent Security Graph providers that enable your app to retrieve alerts and update alert lifecycle properties|
|Microsoft Teams|Microsoft Teams is a platform that combines workplace chat, meetings, notes, and attachmentsQuick Guide: you must first register your app at Microsoft App Registration Portal, Configure Microsoft Teams Integration, Run the action 'Get Authorization', Run the action 'Generate Token'.|
|Palo Alto Cortex XDR|Cortex XDR - XDR is the world’s first detection and response app that natively integrates network, endpoint and cloud data to stop sophisticated attacks.  Cortex XDR accurately detects threats with behavioral analytics and reveals the root cause to speed up investigations.|
|TemplateEngine|Template Engine integration provides the ability to render templates using Jinja2. Jinja2 provide fast and flexible ways to create rich templates. These templates can be used in entity insights, emails, ticketing systems, or any action that can take in a text string.Jinja2 documentation can be found at https://jinja.palletsprojects.com/en/2.11.x/|


## Connectors
|Name|Description|Has Mappings|
|----|-----------|------------|
|Palo Alto Cortex XDR Connector|Pull incidents from Palo Alto XDR. Dynamic List works with the “source” parameter.|False|


## Playbooks
|Name|Description|
|----|-----------|
|AWS EC2 Containment|This block allows the playbook to automatically stop EC2 instances that were identified in the alert as potentially compromised or suspicious, supporting the containment phase of the incident response process.|
|AWS EC2 Enrichment|This block retrieves EC2 instance data associated with the case and provides context for other actions or analysis.|
|AWS Enrichment|This block retrieves EC2 instance data associated with the case and provides context for other actions or analysis.|
|AWS Users Containment|An embedded workflow that can receive inputs and return an output.|
|Amazon Web Services Cloud Platform Starting Playbook|Amazon Web Services Cloud Platform Starting Playbook provides reference implementation of how Amazon Web Services Cloud Platform alerts can be processed in Google SecOps.|
|Azure Containment|This block allows the playbook to apply containment actions to Azure user accounts by either updating the password or disabling the account. It also provides the option to ignore the action and take no changes when required.|
|Azure Containment - 1|This block allows the playbook to apply containment actions to Azure user accounts by either updating the password or disabling the account. It also provides the option to ignore the action and take no changes when required.|
|Azure Enrichment|This block enriches Siemplify Host and User entities with relevant information from Azure Active Directory, providing additional context to support investigation and response activities.|
|Azure Enrichment - 1|This block enriches Siemplify Host and User entities with relevant information from Azure Active Directory, providing additional context to support investigation and response activities.|
|CrowdStrike Containment|This block allows the playbook to perform containment actions on endpoints by targeting the IPs and hostnames associated with the case, helping to prevent further compromise during incident response.|
|CrowdStrike Falcon Starting Playbook|CrowdStrike Falcon Starting Playbook provides reference implementation of how CrowdStrike Falcon alerts can be processed in Google SecOps.|
|GTI Enrichment|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|GTI Enrichment - 1|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|GTI Enrichment - 2|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|GTI Enrichment - 3|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|GTI Enrichment - 4|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|GTI Enrichment - 5|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|GTI Enrichment - 6|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|GTI Enrichment - 7|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|Google SecOps Enrichment|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Google SecOps Enrichment - 1|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Google SecOps Enrichment - 2|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Google SecOps Enrichment - 3|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Google SecOps Enrichment - 4|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Google SecOps Enrichment - 5|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Google SecOps Enrichment - 6|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Google SecOps Enrichment - 7|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Google Workspace Containment|This block allows the playbook to update Google Workspace Directory user accounts as part of containment or response actions, supporting account management and security controls.|
|Google Workspace Enrichment|This block enriches user entities with relevant information from Google Workspace, providing additional context to support investigation and response activities.|
|Google Workspace Enrichment - 1|This block enriches user entities with relevant information from Google Workspace, providing additional context to support investigation and response activities.|
|Google Workspace Enrichment - 2|This block enriches user entities with relevant information from Google Workspace, providing additional context to support investigation and response activities.|
|Google Workspace Enrichment - 3|This block enriches user entities with relevant information from Google Workspace, providing additional context to support investigation and response activities.|
|Google Workspace Starting Playbook|Google Workspace Starting Playbook provides reference implementation of how Google Workspace alerts can be processed in Google SecOps.|
|High Risk Users Check|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|High Risk Users Check - 1|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|High Risk Users Check - 2|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|High Risk Users Check - 3|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|High Risk Users Check - 4|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|High Risk Users Check - 5|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|MITRE Enrichment|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|MITRE Enrichment - 1|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|MITRE Enrichment - 2|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|MITRE Enrichment - 3|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|MITRE Enrichment - 4|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|MITRE Enrichment - 5|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|MITRE Enrichment - 6|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|Microsoft Azure Cloud Platform Starting Playbook|Microsoft Azure Cloud Platform Starting Playbook provides reference implementation of how Microsoft Azure Cloud Platform alerts can be processed in Google SecOps.|
|Microsoft Azure Cloud Platform Starting Playbook - 1|Microsoft Azure Cloud Platform Starting Playbook provides reference implementation of how Microsoft Azure Cloud Platform alerts can be processed in Google SecOps.|
|Microsoft Defender For Endpoint Containment|This block allows the playbook to create an isolate machine task in Microsoft Defender for Endpoint, helping to contain affected systems and prevent further network communication.|
|Microsoft Defender For Endpoint Containment - 1|This block allows the playbook to create an isolate machine task in Microsoft Defender for Endpoint, helping to contain affected systems and prevent further network communication.|
|Microsoft Defender For Endpoint Enrichment|This block enriches Microsoft Defender for Endpoint hosts by retrieving relevant data such as logged-on users, file-related alerts, and machine-related alerts. It also supports file enrichment using SHA1 hashes, providing additional context to assist investigation and response activities.|
|Microsoft Defender For Endpoint Enrichment - 1|This block enriches Microsoft Defender for Endpoint hosts by retrieving relevant data such as logged-on users, file-related alerts, and machine-related alerts. It also supports file enrichment using SHA1 hashes, providing additional context to assist investigation and response activities.|
|Microsoft Defender for Endpoint Starting Playbook|Microsoft Defender for Endpoint Starting Playbook provides reference implementation of how Microsoft Defender for Endpoint alerts can be processed in Google SecOps.|
|Microsoft Defender for Endpoint Starting Playbook - 1|Microsoft Defender for Endpoint Starting Playbook provides reference implementation of how Microsoft Defender for Endpoint alerts can be processed in Google SecOps.|
|Okta Enrichment|This block retrieves information about a user from Okta, including all roles assigned to the user and the groups the user is a member of, providing additional context for analysis and response actions.|
|Okta Remediation Block|This block allows the playbook to perform remediation actions on Okta users, including generating a one-time token to reset a user’s password, disabling the user, or taking no action as needed.|
|Okta Starting Playbook|Okta Starting Playbook provides reference implementation of how Okta alerts can be processed in Google SecOps.|
|New Playbook||


## Visual Families
|Name|Description|
|----|-----------|
|Test1|testing|


## Jobs
|Name|Description|
|----|-----------|
|Google Chronicle Alerts Creator Job|This job will sync new SOAR alerts with Chronicle SIEM.Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.|

