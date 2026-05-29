
# QualysVM

Qualys VM (Vulnerability Management) is a cloud-based service that gives you immediate, global visibility into where your IT systems might be vulnerable to the latest Internet threats and how to protect them. It helps you to continuously identify threats and monitor unexpected changes in your network before they turn into breaches.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root||True|String||
|Username||True|String||
|Password||True|Password|*****|
|X-Requested-With Header|On behalf of whom, the API requests need to be executed in the integration|True|String|Google SecOps SOAR|
|Verify SSL||False|Boolean|False|


#### Dependencies
| |
|-|
|certifi-2026.4.22-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|xmltodict-0.13.0-py2.py3-none-any.whl|
|EnvironmentCommon-1.0.1-py2.py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|TIPCommon-1.0.12-py2.py3-none-any.whl|
|idna-3.13-py3-none-any.whl|


## Actions
#### Launch Scan Report
Launch a scan report
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Report Title|A user-defined report title. The title may have a maximum of 128 characters. For a PCI compliance report, the report title is provided by Qualys and cannot be changed.|True|String||
|Report Type|Template name. For example: Technical Report.|True|String||
|Output Format|One output format may be specified. When output_format=pdf is specified, the Secure PDF Distribution may be used. e.g: pdf, mht and html.|True|String||
|IPs/Ranges|Specify IPs/ranges to change (override) the report target, as defined in the patch report template. Multiple IPs/ranges are comma separated.|False|String||
|Asset Groups|Asset groups.if more than one has to be comma separated.|False|String||
|Scan Reference|For a PCI compliance report, either the technical or executive report, this parameter specifies the scan reference to include. A scan reference starts with the string "scan/" followed by a reference ID number. The scan reference must be for a scan that was run using the PCI Options profile. Only one scan reference may be specified.|False|String||



#### Launch Compliance Report
Launch a compliance report
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Report Title|A user-defined report title. The title may have a maximum of 128 characters. For a PCI compliance report, the report title is provided by Qualys and cannot be changed.|True|String||
|Report Type|Template name. For example: Qualys Top 20 Report, Payment Card Industry (PCI).|True|String||
|Output Format|One output format may be specified. When output_format=pdf is specified, the Secure PDF Distribution may be used. e.g: pdf, mht and html.|True|String||
|IPs/Ranges|Specify IPs/ranges to change (override) the report target, as defined in the patch report template. Multiple IPs/ranges are comma separated.|False|String||
|Asset Groups|Asset groups.if more than one has to be comma separated.|False|String||
|Scan Reference|Show only a scan with a certain scan reference code.|False|String||



#### Enrich Host
Enrich host with information from Qualys VM. Note: AssetView module is required. Supported entities: IP Address, Hostname.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Create Insight|If enabled, action will create an insight containing all of the retrieved information about the entity.|False|Boolean|true|



#### Download Report
Fetch report by ID
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Report ID|Report ID value.|True|String||



#### Download Vm Scan Results
Fetch vulnerability scan results by scan id.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Scan ID|Scan ID value. Scan ID format: scan/{integer}.{integer}|True|String||



#### List Endpoint Detections
List endpoint detections in Qualys VM. Supported entities: IP Address, Hostname.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Status Filter|Specify a comma-separated list of statuses that should be used during ingestion. If nothing is provided, the action will ingest detections with New, Active, Re-Opened statuses. Possible values: New, Active, Re-Opened, Fixed|False|String|New, Active, Re-Opened|
|Lowest Severity To Fetch|Specify the lowest severity that will be used to fetch detections.|False|List|Medium|
|Max Detections To Return|Specify how many detections to return per entity. Default: 50. Maximum: 200.|False|String|50|
|Ingest Ignored Detections|If enabled, action will also return ignored detections.|False|Boolean|false|
|Ingest Disabled Detections|If enabled, action will also return disabled detections.|False|Boolean|false|
|Create Insight|If enabled, action will create an insight containing information about vulnerabilities found on the entity.|False|Boolean|true|



#### Launch Patch Report
Launch a patch report
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Report Title|A user-defined report title. The title may have a maximum of 128 characters. For a PCI compliance report, the report title is provided by Qualys and cannot be changed.|True|String||
|Report Type|Template name. For example: Qualys Patch Report.|True|String||
|Output Format|One output format may be specified. When output_format=pdf is specified, the Secure PDF Distribution may be used. e.g: pdf, online, xml or csv.|True|String||
|IPs/Ranges|Specify IPs/ranges to change (override) the report target, as defined in the patch report template. Multiple IPs/ranges are comma separated.|False|String||
|Asset Groups|Asset groups.if more than one has to be comma separated.|False|String||



#### List Reports
List of reports in the user's account when Report Share feature is enabled. The report list output includes all report types, including scorecard reports. 
Timeout - 600 Seconds



#### Launch VM Scan And Fetch Results
Launch vulnerability scan on a host in your network and fetch results. NOTICE! This action will automatically new hosts to Qualys as assets. Please note that your license limit number of hosts depends on your subscription. Supported entities: IP Address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Title|The scan title. This can be a maximum of 2000 characters (ascii)|False|String||
|Processing Priority|Specify a value of 0 - 9 to set a processing priority level for the scan. When not specified, a value of 0 (no priority) is used. Valid values are: 0 for No Priority (the default), 1 for Emergency, 2 for Ultimate,3 for Critical, 4 for Major, 5 for High, 6 for Standard 7 for Medium, 8 for Minor and 9 for Low|True|String||
|Scan Profile|The title of the compliance option profile to be used. One of these parameters must be specified in a request: option_title or option_id. For example: Qualys Top 20 Options.|True|String||
|Scanner Appliance|The friendly names of the scanner appliances to be used or "External" for external scanners. Multiple entries are comma separated.|False|String||
|Network|The ID of a network used to filter the IPs/ranges specified in the "ip" parameter. Set to a custom network ID (note this does not filter IPs/ranges specified in "asset_groups" or "asset_group_ids"). Or set to "0" (the default) for the Global Default Network - this is used to scan hosts outside of your custom networks.|False|String||



#### List Ips
List IP addresses in the user's account. By default, all hosts in the user's account are included.
Timeout - 600 Seconds



#### Launch Remediation Report
Launch a remediation report
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Report Title|A user-defined report title. The title may have a maximum of 128 characters. For a PCI compliance report, the report title is provided by Qualys and cannot be changed.|True|String||
|Report Type|Template name. For example: Tickets per Asset Group, Tickets per Vulnerability.|True|String||
|Output Format|One output format may be specified. When output_format=pdf is specified, the Secure PDF Distribution may be used. e.g: pdf, mht and html.|True|String||
|IPs/Ranges|Specify IPs/ranges to change (override) the report target, as defined in the patch report template. Multiple IPs/ranges are comma separated.|False|String||
|Asset Groups|Asset groups.if more than one has to be comma separated.|False|String||
|Display Results For All tickets|Specifies whether the report will include tickets assigned to the current user (User is set by default), or all tickets in the user account. By default tickets assigned to the current user are included.|False|Boolean|false|



#### List Groups
List asset groups in the user's account.
Timeout - 600 Seconds



#### List Scans
List of scans launched within the past 30 days.
Timeout - 600 Seconds



#### Ping
Test Connectivity
Timeout - 600 Seconds









## Connectors
#### Qualys VM - Detections Connector
Pull detections from Qualys VM. Note: whitelist works with "Type" parameter.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|API Root|API Root of the Qualis VM instance.|True|String||
|Username|Username of the Qualis VMDR instance.|True|String||
|Password|Password of the Qualis VMDR instance.|True|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Qualys VM server is valid.|False|Boolean|true|
|Lowest Severity To Fetch|Lowest severity that will be used to fetch detections. If nothing is provided, the connector will fetch all detections. Maximum: 5.|False|Int|1|
|Status Filter|Status filter for the connector. If nothing is provided, the connector will ingest detections with "New, Active, Re-Opened" statuses. Possible values: NEW, ACTIVE, FIXED, RE-OPENED.|False|String|NEW, ACTIVE, RE-OPENED|
|Ingest Ignored Detections|If enabled, the connector will ingest ignored detections.|False|Boolean|false|
|Ingest Disabled Detections|If enabled, the connector will ingest disabled detections.|False|Boolean|false|
|Grouping Mechanism|Grouping mechanism that will be used to create Siemplify Alerts. Possible values: Host, Detection, None. If Host is provided, the connector will create 1 Siemplify alert containing all of the detection related to the host. If Detection is provided, the connector will create 1 Siemplify Alert containing information about all of the hosts that have that detection. If None or invalid value is provided, the connector will create a new Siemplify alert for each separate detection per host.|True|String|Detection|
|Use whitelist as a blacklist|If enabled, whitelist will be used as a blacklist.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|
|X-Requested-With Header|On behalf of whom, the API requests need to be executed in the integration|True|String|Google SecOps SOAR|




