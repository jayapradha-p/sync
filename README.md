# GitSync

## Integrations
|Name|Description|
|----|-----------|
|Abnormal Security|Abnormal Security uses AI to protect organizations from email attacks. This integration enables automated ingestion of threats and cases as SOAR alerts, plus search and remediation of malicious email messages through the Abnormal Security API. For support, contact: support@abnormalsecurity.com|
|Active Directory|Microsoft Active Directory integration facilitates the centralized management and synchronization of Windows user accounts with Security Center's administrator and cardholder accounts.|
|AlgoSec|Manage your network security effectively, swiftly, and confidently. No matter where your network lives. Gain complete visibility, automate changes, and always be compliant.|
|AlienVault USM Appliance|USM Appliance includes the essential security capabilities and continuously delivered threat intelligence needed to quickly and easily identify and respond to threats in your physical and virtual infrastructure.|
|Anomali|Anomali ThreatStream operationalizes threat intelligence, automating collection and integration, and enabling security teams to analyze and respond to threats.|
|Automox|Automox is the modern, cloud-native endpoint-hardening platform that empowers organizations to remediate vulnerabilities faster than they can be weaponized.|
|Certly|Determining whether or not a domain or link is malicious.|
|CyberX|The most widely-deployed ICS, SCADA & IIoT security platform that continuously reduces OT network risk via ICS threat monitoring & asset discovery.|
|Cybersixgill DVE Feed|The Cybersixgill Dynamic Vulnerability Exploit (DVE) Score is based on the most comprehensive collection of vulnerability-related threat intelligence and is the only solution that provides users total context and predicts the immediate risks of a vulnerability based on threat actorsâ€™ intent. Google SecOps users can track threats stemming from CVEs that most others define as irrelevant and have a higher probability of being exploited via Google SecOpsâ€™s dashboard.|
|Cybersixgill Darkfeed|Powered by the broadest, automated collection from the deep and dark web, Cybersixgill Darkfeed is a feed of malicious indicators of compromise (IOCs), including domains, URLs, hashes and IP addresses. IOCs are automatically extracted and delivered in real-time, and it is actionable, allowing Google SecOps customers to receive and preemptively block items that threaten their organization.|
|DShield|DShield is a community-based collaborative firewall log correlation system. It receives logs from volunteers worldwide and uses them to analyze attack trends.|
|EasyVista|Radically simplify and accelerate service creation, deployment, and support with  proven and integrated ITSM platform.|
|Elastica Cloud SOC|Security Operations Center for cloud apps that provides full life cycle of security for SaaS.|
|Google Chronicle|Google SecOps enables you to examine the aggregated security information for your enterprise going back for months or longer. Use Google SecOps to search across all of the domains accessed from within your enterprise. To enable the Google API client to communicate with the Backstory API you will need Google Developer Service Account Credential, https://developers.google.com/identity/protocols/OAuth2#serviceaccount.|
|Google SecOps AI Agents|This integration provides first-party AI agents for Google Chronicle. It allows users to leverage Google's advanced AI capabilities for security operations and threat intelligence within the Chronicle platform.|
|IPVoid|IPVoid offers a vast range of IP address tools to discover details about IP addresses.IP blacklist check, whois lookup, dns lookup, ping, and more!|
|Proofpoint Email Protection|Proofpoint Email Protection stops malware and non-malware threats such as impostor email (also known as email fraud).|
|SentinelOne|Endpoint security software that defends every endpoint against every type of attack, at every stage in the threat lifecycle.|
|ThreatCrowd|ThreatCrowd is a system for finding and researching artifacts relating to cyber threats.|


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
|projects/project/locations/location/instances/instance/integrations/CrowdStrikeFalcon/jobs/781/jobInstances/67|This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.|
|projects/project/locations/location/instances/instance/integrations/PaloAltoCortexXDR/jobs/787/jobInstances/68|This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.|

