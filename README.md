# GitSync

## Integrations
|Name|Description|
|----|-----------|
|AWS Cloud Trail|AWS CloudTrail is a service that enables governance, compliance, operational auditing, and risk auditing of your AWS account. With CloudTrail, you can log, continuously monitor, and retain account activity related to actions across your AWS infrastructure. CloudTrail provides event history of your AWS account activity, including actions taken through the AWS Management Console, AWS SDKs, command line tools, and other AWS services. This event history simplifies security analysis, resource change tracking, and troubleshooting. In addition, you can use CloudTrail to detect unusual activity in your AWS accounts. These capabilities help simplify operational analysis and troubleshooting.|
|AWS GuardDuty|Amazon GuardDuty informs you of the status of your AWS environment by producing security findings. GuardDuty helps to detect and manage threats to your AWS system.|
|AWS IAM Access Analyzer|AWS IAM Access Analyzer is built on Zelkova, which translates IAM policies into equivalent logical statements, and runs a suite of general-purpose and specialized logical solvers (satisfiability modulo theories) against the problem. Access Analyzer applies Zelkova repeatedly to a policy with increasingly specific queries to characterize classes of behaviors the policy allows, based on the content of the policy. To learn more about satisfiability modulo theories, see Satisfiability Modulo Theories. Access Analyzer does not examine access logs to determine whether an external entity accessed a resource within your zone of trust. It generates a finding when a resource-based policy allows access to a resource, even if the resource was not accessed by the external entity. Access Analyzer also does not consider the state of any external accounts when making its determination. That is, if it indicates that account 11112222333 can access your S3 bucket, it knows nothing about the state of users, roles, service control policies (SCP), and other relevant configurations in that account. This is for customer privacy – Access Analyzer doesn't consider who owns the other account. It is also for security – if the account is not owned by the Access Analyzer customer, it is still important to know that an external entity could gain access to their resources even if there are currently no principals in the account that could access the resources. Access Analyzer considers only certain IAM condition keys that external users cannot directly influence, or that are otherwise impactful to authorization. Access Analyzer does not currently report findings from AWS service principals or internal service accounts. In rare cases where Access Analyzer isn't able to fully determine whether a policy statement grants access to an external entity, it errs on the side of declaring a false positive finding. Access Analyzer is designed to provide a comprehensive view of the resource sharing in your account, and strives to minimize false negatives.|
|AWS Security Hub|AWS Security Hub gives you a comprehensive view of your high-priority security alerts and security posture across your AWS accounts. There are a range of powerful security tools at your disposal, from firewalls and endpoint protection to vulnerability and compliance scanners. But oftentimes this leaves your team switching back-and-forth between these tools to deal with hundreds, and sometimes thousands, of security alerts every day.|
|AbuseIPDB|Leverage the AbuseIPDB threat intelligence API with this integration.|
|AirTable|Airtable can store information in a spreadsheet that's visually appealing and easy-to-use, but it's also powerful enough to act as a database that businesses can use for customer-relationship management (CRM), task management, project planning, and tracking inventory.|
|AlienVault USM Anywhere|AlienVault USM Anywhere delivers powerful threat detection, incident response, and compliance management for cloud, on-premises, and hybrid environments.|
|Amazon Macie|Amazon Macie is a powerful security and compliance service that provides an automatic method to detect, identify, and classify data within your AWS account.|
|Arcsight|Real-time threat detection and automated response backed by a powerful, open, and intelligent SIEM (Security Information and Event Management).|
|Azure Security Center|Azure Security Center is a unified infrastructure security management system that strengthens the security posture of your data centers, and provides advanced threat protection across your hybrid workloads in the cloud - whether they're in Azure or not - as well as on premises.|
|Vmware Carbon Black Cloud|The VMware Carbon Black Cloud is a cloud-native endpoint protection platform (EPP) that combines the intelligent system hardening and behavioral prevention needed to keep emerging threats at bay, using a single lightweight agent, and an easy-to-use console.|
|CrowdStrike Falcon|CrowdStrike Falcon is the leader in next-generation endpoint protection, threat intelligence and incident response through cloud-based endpoint protection.|
|Functions|A set of math and data manipulation actions created for Google SecOps Community to power up playbook capabilities.|
|Google Chronicle|Google SecOps enables you to examine the aggregated security information for your enterprise going back for months or longer. Use Google SecOps to search across all of the domains accessed from within your enterprise. To enable the Google API client to communicate with the Backstory API you will need Google Developer Service Account Credential, https://developers.google.com/identity/protocols/OAuth2#serviceaccount.|
|Microsoft Azure Sentinel|Microsoft Azure Sentinel is a scalable, cloud-native, security information event management (SIEM) and security orchestration automated response (SOAR) solution. Azure Sentinel delivers intelligent security analytics and threat intelligence across the enterprise, providing a single solution for alert detection, threat visibility, proactive hunting, and threat response.|
|Microsoft Graph Mail|Microsoft 365 and Office 365 deliver the power of cloud productivity to businesses of all sizes, helping save time, money, and free up valued resources. The Microsoft 365 and Office 365 plans combine the familiar Microsoft Office desktop suite with cloud-based versions of Microsoft's next-generation communications and collaboration services (including Office for the web, Microsoft Exchange Online, Microsoft Teams, and Microsoft SharePoint Online) to help users be productive from virtually anywhere through the Internet. This integration uses Microsoft Graph Mail API to communicate with Microsoft 365 and Office 365 services.|
|Microsoft Graph Mail Delegated|This integration version uses Delegated Authentication in Microsoft 365 and requires interactive login of the user on behalf of which integration should communicate with Microsoft 365. To configure this integration, provide all parameters except for Refresh Token, and save the integration configuration, then run “Get Authorization” and “Generate Token” actions to get the token and then provide it in integration configuration to finish the process. Microsoft 365 and Office 365 deliver the power of cloud productivity to businesses of all sizes, helping save time, money, and free up valued resources. The Microsoft 365 and Office 365 plans combine the familiar Microsoft Office desktop suite with cloud-based versions of Microsoft's next-generation communications and collaboration services (including Office for the web, Microsoft Exchange Online, Microsoft Teams, and Microsoft SharePoint Online) to help users be productive from virtually anywhere through the Internet. This integration uses Microsoft Graph Mail API to communicate with Microsoft 365 and Office 365 services.|
|Microsoft Teams|Microsoft Teams is a platform that combines workplace chat, meetings, notes, and attachmentsQuick Guide: you must first register your app at Microsoft App Registration Portal, Configure Microsoft Teams Integration, Run the action 'Get Authorization', Run the action 'Generate Token'.|
|Palo Alto Cortex XDR|Cortex XDR - XDR is the world’s first detection and response app that natively integrates network, endpoint and cloud data to stop sophisticated attacks.  Cortex XDR accurately detects threats with behavioral analytics and reveals the root cause to speed up investigations.|
|SentinelOneV2|Endpoint security software that defends every endpoint against every type of attack, at every stage in the threat lifecycle.|
|Tools|A set of utility actions for data manipulation and common platform tasks to power up playbook capabilities.|
|VirusTotalV3|VirusTotal was founded in 2004 as a free service that analyzes files and URLs for viruses, worms, trojans and other kinds of malicious content. Our goal is to make the internet a safer place through collaboration between members of the antivirus industry, researchers and end users of all kinds. Fortune 500 companies, governments and leading security companies are all part of the VirusTotal community, which has grown to over 500,000 registered users.This integration was created using the 3rd iteration of VT API.|


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
|AWS Instance Containment|This block allows you to stop EC2 instances that were identified in the alert as potentially compromised or suspicious, supporting the containment phase of the incident response process.It uses a boolean input to control manual or automatic execution and returns the containment result, false on failure, or an empty value if no action is taken.|
|AWS Users Containment|An embedded workflow that can receive inputs and return an output.|
|Amazon Web Services Cloud Platform Starting Playbook|Amazon Web Services Cloud Platform Starting Playbook provides reference implementation of how Amazon Web Services Cloud Platform alerts can be processed in Google SecOps.|
|Clean Case|Clean case (Tags, Alert scoring info, etc) when playbooks that are often rerun and can create duplicate evidence.  Extend this logic to meet your requirements.|
|Duplicate Alert Check|Is this Alert the first in the Case?  Is it the first in the Case of this Alert type?  Or is it a duplication.  Example usage: this Block can be used when Alert Grouping is causing multiple ITSM tickets for the same case. Different paths output string that can be used in the parent playbook to check the verdict.|
|GCP Instance Containment|This block stops running GCP Compute VM instances, shutting them down gracefully and allowing them to be restarted later if needed. It uses a boolean input to control manual or automatic execution and returns the containment result, false on failure, or an empty value if no action is taken.|
|GCP Instance Containment - 1|This block stops running GCP Compute VM instances, shutting them down gracefully and allowing them to be restarted later if needed. It uses a boolean input to control manual or automatic execution and returns the containment result, false on failure, or an empty value if no action is taken.|
|GCP Service Account Containment|This block disables one or more GCP service accounts as part of containment actions. It uses a boolean input to control manual or automatic execution and returns the containment result, false on failure, or an empty value if no action is taken.|
|GTI Enrichment|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|GTI Enrichment - 1|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|GTI Enrichment - 2|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|GTI Enrichment - 3|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|GTI Enrichment - 4|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|Google Cloud Compute Enrichment|This block provides additional context about GCP Compute resources related to the case, helping the playbook gain relevant information for analysis and response actions.|
|Google SecOps Enrichment|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Google SecOps Enrichment - 1|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Google SecOps Enrichment - 2|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Google SecOps Enrichment - 3|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Google SecOps Enrichment - 4|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Google SecOps SIEM Enrichment|This block enriches entities and retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Google SecOps SIEM Enrichment - 1|This block enriches entities and retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Google Workspace Enrichment|This block enriches user entities with relevant information from Google Workspace, providing additional context to support investigation and response activities.|
|Google Workspace Enrichment - 1|This block enriches user entities with relevant information from Google Workspace, providing additional context to support investigation and response activities.|
|Google Workspace Enrichment - 2|This block enriches user entities with relevant information from Google Workspace, providing additional context to support investigation and response activities.|
|High Risk Users Check|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|High Risk Users Check - 1|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|High Risk Users Check - 2|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|High Risk Users Check - 3|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
|MITRE|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and potential defensive actions. It receives an Add Tag boolean input; when set to true, it adds the MITRE technique ID to the case.|
|MITRE Enrichment|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|MITRE Enrichment - 1|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|MITRE Enrichment - 2|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|MITRE Enrichment - 3|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|Microsoft Defender For Endpoint Containment|This block allows the playbook to create an isolate machine task in Microsoft Defender for Endpoint, helping to contain affected systems and prevent further network communication.|
|Microsoft Defender For Endpoint Enrichment|This block enriches Microsoft Defender for Endpoint hosts by retrieving relevant data such as logged-on users, file-related alerts, and machine-related alerts. It also supports file enrichment using SHA1 hashes, providing additional context to assist investigation and response activities.|
|Microsoft Defender for Endpoint Starting Playbook|Microsoft Defender for Endpoint Starting Playbook provides reference implementation of how Microsoft Defender for Endpoint alerts can be processed in Google SecOps.|
|Okta Containment|This block performs remediation on Okta users by generating a one‑time token for password resets or disabling accounts. A boolean input controls manual or automatic mode. In automatic mode, the Disable Account and Password Reset flags determine which actions run. It returns the remediation result, false on failure, or empty if no action is taken.|
|Proofpoint Enrichment|This block uses the List Campaigns action to retrieve a list of active campaigns in Proofpoint TAP, providing relevant information to support investigation and threat analysis activities.|
|Salesforce Starting Playbook|Salesforce Starting Playbook provides reference implementation of how Salesforce alerts can be processed in Google SecOps|
|Salesforce Starting Playbook - 1|Salesforce Starting Playbook provides reference implementation of how Salesforce alerts can be processed in Google SecOps|
|Sentinel One Containment|This block filters the relevant entities and performs containment actions in SentinelOne, including adding hashes to a blacklist and disconnecting the endpoint agent from the network using its hostname or IP address.|
|Sentinel One Enrichment|This block retrieves information about endpoints from SentinelOne, including details by IP address or hostname, available applications on the endpoint, and associated hashes, providing additional context to support analysis and response activities.|
|SentinelOne Starting Playbook|SentinelOne Starting Playbook provides reference implementation of how SentinelOne alerts can be processed in Google SecOps.|
|Symantec Enrichment|This block supports remediation by retrieving system information for endpoints and listing all endpoints/sensors and groups configured on a specified Symantec-managed device, providing the necessary context for follow-up actions. It receives a boolean Scan Endpoint input; when set to true, the endpoint will be scanned.|
|Symantec Enrichment - 1|This block supports remediation by retrieving system information for endpoints and listing all endpoints/sensors and groups configured on a specified Symantec-managed device, providing the necessary context for follow-up actions. It receives a boolean Scan Endpoint input; when set to true, the endpoint will be scanned.|
|Tag Case with time span|A Block that Tags the case with the time span between Alerts.  Can be used for Case queue filters.|
|Zscaler Containment|This block allows you to add a URL, domain, or IP address to the Zscaler blacklist as part of containment actions, helping prevent further access to potentially harmful resources. It uses a boolean input to control manual or automatic execution and returns the containment result, false on failure, or an empty value if no action is taken.|
|Zscaler Containment - 1|This block allows you to add a URL, domain, or IP address to the Zscaler blacklist as part of containment actions, helping prevent further access to potentially harmful resources. It uses a boolean input to control manual or automatic execution and returns the containment result, false on failure, or an empty value if no action is taken.|
|New Playbook - 1||
|New Playbook - 10||
|New Playbook - 11||
|New Playbook - 12||
|New Playbook - 13||
|New Playbook - 14||
|New Playbook - 15||
|New Playbook - 2||
|New Playbook - 3||
|New Playbook - 4||
|New Playbook - 5||
|New Playbook - 6||
|New Playbook - 7||
|New Playbook - 8||
|New Playbook - 9||
|Copy of New Playbook - 1||
|Copy of New Playbook - 10||
|Copy of New Playbook - 11||
|Copy of New Playbook - 12||
|Copy of New Playbook - 13||
|Copy of New Playbook - 14||
|Copy of New Playbook - 15||
|Copy of New Playbook - 2||
|Copy of New Playbook - 3||
|Copy of New Playbook - 4||
|Copy of New Playbook - 5||
|Copy of New Playbook - 6||
|Copy of New Playbook - 7||
|Copy of New Playbook - 8||
|Copy of New Playbook - 9||
|Copy of New Playbook - 1 - 2||
|New Block|An embedded workflow that can receive inputs and return an output.|
|New Block - 10|An embedded workflow that can receive inputs and return an output.|
|New Block - 12|An embedded workflow that can receive inputs and return an output.|
|New Block - 2|An embedded workflow that can receive inputs and return an output.|
|New Block - 3|An embedded workflow that can receive inputs and return an output.|
|New Block - 4|An embedded workflow that can receive inputs and return an output.|
|New Block - 5|An embedded workflow that can receive inputs and return an output.|
|New Block - 6|An embedded workflow that can receive inputs and return an output.|
|New Block - 7|An embedded workflow that can receive inputs and return an output.|
|New Block - 8|An embedded workflow that can receive inputs and return an output.|
|New Block - 9|An embedded workflow that can receive inputs and return an output.|


## Jobs
|Name|Description|
|----|-----------|
|Google Chronicle Alerts Creator Job|This job will sync new SOAR alerts with Chronicle SIEM.Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.|
|Refresh Token Renewal Job|Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.|
|Sync Incidents - 1|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|
|Sync Incidents - 1hhjhjjhhj|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|
|Sync Incidents|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|

