# GitSync

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

