
# Censys

Strengthen your security posture by integrating Censys with Google SecOps SOAR. This integration enables automated threat intelligence workflows, faster incident investigation through rich contextual insights from your Censys environment. Support Contact: support@censys.com

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Key|Censys API Key.|True|Password|*****|
|Organization Id|Censys Organization ID.|True|String||
|Verify SSL|Verify SSL|False|Boolean|false|


#### Dependencies
| |
|-|
|pyopenssl-26.0.0-py3-none-any.whl|
|certifi-2026.2.25-py3-none-any.whl|
|google_api_python_client-2.193.0-py3-none-any.whl|
|proto_plus-1.27.2-py3-none-any.whl|
|pycparser-3.0-py3-none-any.whl|
|charset_normalizer-3.4.6-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|httpx-0.28.1-py3-none-any.whl|
|google_api_core-2.30.1-py3-none-any.whl|
|httpcore-1.0.9-py3-none-any.whl|
|uritemplate-4.2.0-py3-none-any.whl|
|pyparsing-3.3.2-py3-none-any.whl|
|h11-0.16.0-py3-none-any.whl|
|anyio-4.13.0-py3-none-any.whl|
|google_auth_httplib2-0.3.1-py3-none-any.whl|
|requests-2.32.5-py3-none-any.whl|
|google_auth-2.49.1-py3-none-any.whl|
|TIPCommon-2.2.22-py2.py3-none-any.whl|
|googleapis_common_protos-1.73.1-py3-none-any.whl|
|pyasn1_modules-0.4.2-py3-none-any.whl|
|httplib2-0.31.2-py3-none-any.whl|
|EnvironmentCommon-1.0.3-py3-none-any.whl|
|requests_toolbelt-1.0.0-py2.py3-none-any.whl|
|idna-3.11-py3-none-any.whl|
|protobuf-6.33.6-py3-none-any.whl|
|cffi-2.0.0-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.whl|
|urllib3-2.6.3-py3-none-any.whl|
|typing_extensions-4.15.0-py3-none-any.whl|
|pycryptodome-3.23.0-cp37-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|
|cryptography-46.0.6-cp311-abi3-manylinux2014_x86_64.manylinux_2_17_x86_64.whl|
|pyasn1-0.6.3-py3-none-any.whl|


## Actions
#### Enrich Web Properties
This action retrieves comprehensive information about a web property (domain/hostname(IP Address)) using the Censys Platform API. Web properties are identified using a combination of a hostname and port (e.g., platform.censys.io:80). It provides detailed intelligence about web-facing assets including HTTP/HTTPS services, certificates, technologies, and security configurations.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Port|Comma separated ports associated with domain or hostname|True|String|80, 443|
|At Time|RFC3339 Timestamp to view all requested hosts at a specific point in time. Ensure that you suffix the date with T00:00:00Z or a specific time.|False|String||



#### Get Related Infrastructure Results
This action retrieves the detailed pivot results from a completed CensEye job, formats them into a table with 5 columns, and generates Censys search URLs for each pivot. Maximum 50 results per job. Learn more about CensEye in the Censys documentation: https://docs.censys.com/docs/platform-threat-hunting-use-censeye-to-build-detections
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Job ID|The unique identifier of the completed CensEye job.|True|String||



#### Get Rescan Status
This action retrieves the current status of a scan by its ID. It allows users to monitor the progress of previously initiated scans and determine when scan results are available.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Scan ID|The unique identifier of the tracked scan.|True|String||



#### Enrich Certificates
This action retrieves comprehensive information about a single SSL/TLS certificate using the Censys Platform API. A certificate is identified by its SHA-256 fingerprint in the Censys dataset. It provides detailed certificate intelligence including issuer, subject, validity periods, SANs (Subject Alternative Names), and associated hosts.
Timeout - 600 Seconds



#### Get Host History
This action retrieves the event history for a host (IP address). It allows users to view historical scan data, track infrastructure changes over time, and identify when services were added, removed, or modified.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Host ID|The IP address of a host.|True|String||
|Start Time|Start time of the host timeline. Must be a valid RFC3339 string (e.g., 2025-01-01T00:00:00Z). It should be less than the end time.|True|String||
|End Time|End time of the host timeline. Must be a valid RFC3339 string (e.g., 2025-01-02T00:00:00Z). It should be less than the current time.|True|String||



#### Initiate Rescan
This action initiates a live rescan for a known host service at a specific IP and port or hostname and port. The scan may take several minutes to complete and returns a scan ID that can be used to monitor the scan's status.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|IOC Type|Initiate a rescan for a known IP or domain.|True|List|Service|
|IOC Value|IP address or domain name to initiate a rescan.|True|String||
|Port|Port associated with IP or domain. Valid range is 1 to 65535.|True|String|443|
|Protocol|Name of service protocol (Required for SERVICE_ID_OBJECT).|False|String||
|Transport Protocol|Transport Protocol of service (Required for SERVICE_ID_OBJECT).|False|List|Unknown|



#### Create Related Infrastructure Job
This action initiates a CensEye job to discover related infrastructure for a given target (host, web property, or certificate). The job runs asynchronously and returns a job ID that can be used to monitor status and retrieve results. Learn more about CensEye in the Censys documentation: https://docs.censys.com/docs/platform-threat-hunting-use-censeye-to-build-detections
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Target Type|The type of asset to analyze for related infrastructure.|True|List|Host|
|Target Value|The actual value to analyze:- Host: IP address (e.g., "14.84.5.68")- Web Property: domain:port (e.g., "example.com:443")- Certificate: SHA-256 fingerprint (64 hex characters)|True|String||



#### Enrich IPs
This action retrieves comprehensive information about multiple hosts (IP address) using the Censys Platform API. It provides detailed intelligence about internet-facing infrastructure including services, ports, protocols, certificates, vulnerabilities, and location data to help security teams understand their attack surface exposure.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|At Time|RFC3339 Timestamp to view all requested hosts at a specific point in time. Ensure that you suffix the date with T00:00:00Z or a specific time.|False|String||



#### Ping
This action will test the connectivity of the Google SecOps SOAR server to the Censys platform.
Timeout - 600 Seconds



#### Get Related Infrastructure Job Status
This action retrieves the current status of a CensEye job by its ID. It supports async execution and will return IN_PROGRESS status if the job is still running, allowing playbooks to poll until completion. Learn more about CensEye in the Censys documentation: https://docs.censys.com/docs/platform-threat-hunting-use-censeye-to-build-detections
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Job ID|The unique identifier of the CensEye job to check status for.|True|String||









