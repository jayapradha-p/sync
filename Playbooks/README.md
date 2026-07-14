# Playbooks
|Name|Folder|Description|
|----|------|-----------|
|AWS EC2 Containment|Content Hub Playbooks|This block allows the playbook to automatically stop EC2 instances that were identified in the alert as potentially compromised or suspicious, supporting the containment phase of the incident response process.|
|AWS Enrichment|Content Hub Playbooks|This block retrieves EC2 instance data associated with the case and provides context for other actions or analysis.|
|AWS Users Containment|Content Hub Playbooks|An embedded workflow that can receive inputs and return an output.|
|Amazon Web Services Cloud Platform Starting Playbook|Content Hub Playbooks|Amazon Web Services Cloud Platform Starting Playbook provides reference implementation of how Amazon Web Services Cloud Platform alerts can be processed in Google SecOps.|
|BloodHound Attack Path Alerts Playbook|Content Hub Playbooks|Triages BloodHound Enterprise Attack Path alerts ingested via the Attack Paths Alert connector. Resolves involved entities to BloodHound object IDs, checks whether the attack paths still exist, fetches asset metadata, and routes alerts based on environment context for SOC investigation.|
|BloodHound Attack Path Alerts Playbook - 1|Content Hub Playbooks|Triages BloodHound Enterprise Attack Path alerts ingested via the Attack Paths Alert connector. Resolves involved entities to BloodHound object IDs, checks whether the attack paths still exist, fetches asset metadata, and routes alerts based on environment context for SOC investigation.|
|GTI Enrichment|Content Hub Playbooks|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|Google SecOps Enrichment|Content Hub Playbooks|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|MITRE Enrichment|Content Hub Playbooks|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
