
# Rapid7InsightVm

InsightVM vulnerability management software monitors exposures in real-time and adapts to new threats with fresh data, ensuring you can always act at the moment of impact.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root||True|String|https://<host>:<port>/api/3|
|Username||True|String||
|Password||True|Password|*****|
|Verify SSL||False|Boolean|False|


#### Dependencies
| |
|-|
|certifi-2026.4.22-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|arrow-1.4.0-py3-none-any.whl|
|tzdata-2026.2-py2.py3-none-any.whl|
|EnvironmentCommon-1.0.1-py2.py3-none-any.whl|
|python_dateutil-2.9.0.post0-py2.py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|TIPCommon-1.0.12-py2.py3-none-any.whl|
|idna-3.13-py3-none-any.whl|
|six-1.17.0-py2.py3-none-any.whl|


## Actions
#### Enrich Asset
Enrich an asset.
Timeout - 600 Seconds



#### Launch Scan
Start a scan for a specific site.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Scan Engine|The name of the engine to use in the scan.|True|String||
|Scan Name|The scan name.|False|String||
|Scan Template|The name of the template to use in the scan.|True|String||
|Site Name|The name of the site to run the scan on.|True|String||
|Fetch Results|Whether to wait for the scan to complete and get its results or not.|False|Boolean||



#### Get Scan Results
Get scan results by ID
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Scan ID|The ID of the scan.|True|String|None|



#### List Scans
List scans
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Days Backwards|Number of days backwards to fetch scans from.|True|String||



#### Ping
Test Connectivity
Timeout - 600 Seconds









## Connectors
#### Rapid7 InsightVm - Vulnerabilities Connector
Pull information about asset vulnerabilities from Rapid7 InsightVm. Note: whitelist filter works with "protocol" parameter.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|API Root|API root of the Rapid7 InsightVm instance.|True|String|https://{ip}:3780|
|Username|Username of the Rapid7 InsightVm account.|True|String||
|Password|Password of the Rapid7 InsightVm account.|True|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Rapid7 InsightVm server is valid.|False|Boolean|true|
|Lowest Severity To Fetch|Lowest Severity that needs to be used to fetch vulnerabilities. Possible values: Moderate, Severe, Critical. If nothing is provided, the connector will fetch vulnerabilities with all severities.|False|String|Moderate|
|Max Assets To Process|Amount of assets that need to be processed per 1 connector iteration. Note: it’s not recommended to increase the value of this parameter, because the connector will be more prone to timeouts.|False|Int|5|
|Grouping Mechanism|Grouping mechanism that will be used to create Siemplify Alerts. Possible values: Host, None. If Host is provided, the connector will create 1 Siemplify Alert containing all of the vulnerabilities related to the host. If None or invalid value is provided, the connector will create a new Siemplify Alert for each separate vulnerability per host.|True|String|Host|
|Use whitelist as a blacklist|If enabled, whitelist will be used as a blacklist.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




