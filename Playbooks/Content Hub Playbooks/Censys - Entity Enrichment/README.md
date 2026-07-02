# Censys - Entity Enrichment
This playbook automatically enriches IP addresses, domains, and certificate entities with Censys threat intelligence data during alert triage and investigation workflows. It retrieves comprehensive asset information including exposed services, ports, protocols, geolocation, ASN details, and associated infrastructure to provide immediate context for security analysts.



**Enabled:** False

**Version:** 0

**Type:** Playbook

**Priority:** 3

**Playbook Simulator:** False



### Playbook Trigger
**Trigger Type:** Custom Trigger

**Conditions Operator:** Or

##### Conditions
|Key|Operator|Value|
|---|--------|-----|
|[Entity.Type]|Equals|ADDRESS|
|[Entity.Type]|Equals|DOMAIN|
|[Entity.Type]|Equals|FILEHASH|



### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|Enrich Domains|This action retrieves comprehensive information about a web property (domain/hostname(IP Address)) using the Censys Platform API. Web properties are identified using a combination of a hostname and port (e.g., platform.censys.io:80). It provides detailed intelligence about web-facing assets including HTTP/HTTPS services, certificates, technologies, and security configurations.|Censys|Enrich Web Properties|
|Enrich Certificates (SHA256 FILE HASH)|This action retrieves comprehensive information about a single SSL/TLS certificate using the Censys Platform API. A certificate is identified by its SHA-256 fingerprint in the Censys dataset. It provides detailed certificate intelligence including issuer, subject, validity periods, SANs (Subject Alternative Names), and associated hosts.|Censys|Enrich Certificates|
|Enrich IP Addresses|This action retrieves comprehensive information about multiple hosts (IP address) using the Censys Platform API. It provides detailed intelligence about internet-facing infrastructure including services, ports, protocols, certificates, vulnerabilities, and location data to help security teams understand their attack surface exposure.|Censys|Enrich IPs|

