
# TenableSecurityCenter

SecurityCenter is a comprehensive vulnerability analysis solution that provides complete visibility into the security posture of your distributed and complex IT infrastructure. 

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Server Address|The server Address of the Tenable Security Center.|True|IP|None|
|Username|The username of the Tenable Security Center account. Note: Both “Username” and “Password” must be provided.|False|String|None|
|Password|The password of the Tenable Security Center account. Note: Both “Username” and “Password” must be provided.|False|Password|*****|
|Access Key|The Access Key of the Tenable Security Center account. Note: Both “Access Key” and “Secret Key” must be provided.|False|Password|*****|
|Secret Key|The Secret Key of the Tenable Security Center account. Note: Both “Access Key” and “Secret Key” must be provided.|False|Password|*****|
|Use SSL|If selected, the integration validates the SSL certificate when connecting to the Tenable Security Center server. Enabled by default.|False|Boolean|False|


#### Dependencies
| |
|-|
|chardet-5.2.0-py3-none-any.whl|
|requests-2.31.0-py3-none-any.whl|
|certifi-2024.2.2-py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|idna-3.7-py3-none-any.whl|
|TIPCommon-1.0.11-py2.py3-none-any.whl|
|urllib3-1.26.8-py2.py3-none-any.whl|


## Actions
#### Get Scan Results
Wait for scan to complete and get results of the scan
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Scan Result ID|The scan results ID.|True|String||



#### Scan Ips
Initiate a scan of IP addresses
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Scan Name|The name of the scan to create.|True|String||
|Policy Name|The name of the policy.|True|String||



#### Get Report
Get report content by ID or name.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Report ID|Report ID number.Can be found at the report URL.|False|String|None|
|Report Name|The name of the report, as mentioned at the GUI.|False|String|None|



#### Enrich IP
Get information about IP addresses and enrich them
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Repository Name|The repository name.|True|String||



#### Get Related Assets
Get assets that are related to an IP address
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Repository Name|The repository name.|True|String||



#### Add IP To IP List Asset
Add an IP to IP list asset in Tenable.sc.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Asset Name|Specify the name of the IP list asset to which you want to add new IPs.|True|String||



#### Create IP List Asset
Create an IP list asset in Tenable.sc. Requires at least 1 IP entity for successful execution.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Name|Specify the name for the IP list asset.|True|String||
|Description|Specify the description of the IP list asset.|False|String||
|Tag|Specify the tag of the IP list asset.|False|String||



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Get Vulnerabilities for IP
Get vulnerabilities and severity summary for an IP address
Timeout - 600 Seconds



#### Run Asset Scan
Execute Asset Scan in Tenable.sc.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Description|Specify the description for the scan.|False|String||
|Scan Name|Specify the name for the scan.|True|String||
|Asset Name|Specify the name of the asset that should be scanned.|True|String||
|Policy ID|Specify the id of the policy that should be used in the scan.|True|String||
|Repository ID|Specify the id of the repository that should be used in the scan.|True|String||









## Connectors
#### Tenable Security Center Connector
Tenable Security Center Connector

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Server Address|Server Address|True|String||
|Username|Username|False|String||
|Password|Password|False|Password|*****|
|Access Key|Access Key|False|Password|*****|
|Secret Key|Secret Key|False|Password|*****|
|Use SSL|Use SSL|False|Boolean|FALSE|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|
|Max Days Backwards|Specify the amount of days back, from which you would like to fetch data.|False|String|1|
|Limit Per Cycle|Specify the amount of alerts ingested into the connector in each execution cycle.|False|String|10|




