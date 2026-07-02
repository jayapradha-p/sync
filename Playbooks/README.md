# Playbooks
|Name|Folder|Description|
|----|------|-----------|
|AWS EC2 Containment|Content Hub Playbooks|This block allows the playbook to automatically stop EC2 instances that were identified in the alert as potentially compromised or suspicious, supporting the containment phase of the incident response process.|
|AWS Enrichment|Content Hub Playbooks|This block retrieves EC2 instance data associated with the case and provides context for other actions or analysis.|
|AWS Instance Containment|Content Hub Playbooks|This block allows you to stop EC2 instances that were identified in the alert as potentially compromised or suspicious, supporting the containment phase of the incident response process.It uses a boolean input to control manual or automatic execution and returns the containment result, false on failure, or an empty value if no action is taken.|
|AWS Users Containment|Content Hub Playbooks|An embedded workflow that can receive inputs and return an output.|
|Amazon Web Services Cloud Platform Starting Playbook|Content Hub Playbooks|Amazon Web Services Cloud Platform Starting Playbook provides reference implementation of how Amazon Web Services Cloud Platform alerts can be processed in Google SecOps.|
|Censys - Entity Enrichment|Content Hub Playbooks|This playbook automatically enriches IP addresses, domains, and certificate entities with Censys threat intelligence data during alert triage and investigation workflows. It retrieves comprehensive asset information including exposed services, ports, protocols, geolocation, ASN details, and associated infrastructure to provide immediate context for security analysts.|
|GTI Enrichment|Content Hub Playbooks|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|Google SecOps Enrichment|Content Hub Playbooks|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|MITRE Enrichment|Content Hub Playbooks|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|New Playbook|Default||
|New Playbook - 1|Default||
|New Block|New Folder|An embedded workflow that can receive inputs and return an output.|
