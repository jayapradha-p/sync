
# TenableIO

Managed in the cloud and powered by Nessus technology, Tenable.io provides the industry's most comprehensive vulnerability coverage with the ability to predict which security issues to remediate first. It’s your complete end-to-end vulnerability management solution.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|None|True|String|https://cloud.tenable.com|
|Secret Key|None|True|Password|*****|
|Access Key|None|True|Password|*****|
|Verify SSL|None|False|Boolean|True|


#### Dependencies
| |
|-|
|chardet-5.2.0-py3-none-any.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|idna-3.8-py3-none-any.whl|
|EnvironmentCommon-1.0.0-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|
|certifi-2024.8.30-py3-none-any.whl|


## Actions
#### Enrich Entities
Enrich entities using information from Tenable.io. Supported entities: IP Address, Hostname.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Create Insight|If enabled, action will create an insight containing all of the retrieved information about the entity.|False|Boolean|true|



#### Get Vulnerability Details
Retrieve vulnerability details from Tenable.io.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Plugin IDs|Specify a comma-separated list of plugin IDs for which you want to return details.|False|String||
|Create Insight|If enabled, action will create an insight containing information about all of the processed plugin ids.|False|Boolean|true|



#### List Endpoint Vulnerabilities
List endpoint vulnerabilities in Tenable.io. Supported entities: IP Address, Hostname.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Lowest Severity To Fetch|Specify the lowest severity that will be used to fetch vulnerabilities.|False|List|Info|
|Max Vulnerabilities To Return|Specify how many vulnerabilities to return per entity. Default: 50. Maximum: 200.|False|String|50|



#### List Scanners
List available scanners in Tenable.io.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Filter Logic|Specify what filter logic should be applied.|False|List|Equal|
|Filter Value|Specify what value should be used in the filter. If "Equal" is selected, action will try to find the exact match among record types and if "Contains" is selected, action will try to find items that contain that substring. If nothing is provided in this parameter, the filter will not be applied.|False|String||
|Max Scanners To Return|Specify how many scanners to return. Default: 50. Max: 100.|False|String|50|



#### Ping
Test connectivity to the Tenable.io with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### List Policies
List available policies in Tenable.io.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Filter Logic|Specify what filter logic should be applied.|False|List|Equal|
|Filter Value|Specify what value should be used in the filter. If "Equal" is selected, action will try to find the exact match among record types and if "Contains" is selected, action will try to find items that contain that substring. If nothing is provided in this parameter, the filter will not be applied.|False|String||
|Max Policies To Return|Specify how many policies to return. Default: 50. Max: 100.|False|String|50|



#### Scan Endpoints
Initiate a scan on endpoints in Tenable.io. Supported entities: IP Address, Hostname. Note: Action is running as async, please adjust script timeout value in Siemplify IDE for action as needed.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Scan Name|Specify the name of the scan.|True|String||
|Policy Name|Specify the name of the policy that needs to be used for scanning.|True|String||
|Scanner Name|Specify the name of the scanner that should be used. If nothing is provided, action will use the default scanner from configuration.|False|String||
|Send Report To|Specify a comma-separated list of email addresses that need to receive the scan report.|False|String||



#### List Plugin Families
List available plugin families from Tenable.io.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Filter Logic|Specify what filter logic should be applied.|False|List|Equal|
|Filter Value|Specify what value should be used in the filter. If “Equal“ is selected, action will try to find the exact match among record types and if “Contains“ is selected, action will try to find items that contain that substring. If nothing is provided in this parameter, the filter will not be applied.|False|String||
|Max Plugin Families To Return|Specify how many plugin families to return. Default: 50.|False|String|50|









## Connectors
#### TenableIO - Vulnerabilities Connector
Pull vulnerabilities from Tenable.io. Note: connector works with plugin families in whitelist.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|API Root|API Root of the Tenable.io instance.|True|String|https://cloud.tenable.com|
|Access Key|Access Key of the Tenable.io instance.|True|Password|*****|
|Secret Key|Secret Key of the Tenable.io instance.|True|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Tenable.io server is valid.|False|Boolean|true|
|Lowest Severity To Fetch|Lowest severity that will be used to fetch vulnerabilities. If nothing is provided, the connector will fetch all vulnerabilities. Possible values: Info, Low, Medium, High, Critical|False|Int|Medium|
|Status Filter|Status filter for the connector. It works with comma-separated values. If nothing is provided, the connector will ingest vulnerabilities with "open", "reopened" statuses. Possible values: open, reopened, fixed.|False|String|open, reopened|
|Max Days Backwards|Number of days before the first connector iteration to retrieve vulnerabilities from. This parameter applies to the initial connector iteration after you enable the connector for the first time, or used as a fallback value in cases where connector's last run timestamp expires. Default: 30 days. Note: this parameter will return vulnerabilities that were opened/reopened/fixed in the timeframe that is specified in "Max Days Backwards".|False|Int|30|
|Grouping Mechanism|Grouping mechanism that will be used to create Siemplify Alerts. Possible values: Host, Vulnerability, None. If Host is provided, the connector will create 1 Siemplify alert containing all of the vulnerabilities per chunk related to the host. If Vulnerability is provided, the connector will create 1 Siemplify Alert containing information about all of the hosts that have that vulnerability in the scope of 1 chunk. If None or invalid value is provided, the connector will create a new Siemplify alert for each separate vulnerability per host.|True|String|Host|
|Use whitelist as a blacklist|If enabled, whitelist will be used as a blacklist.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




