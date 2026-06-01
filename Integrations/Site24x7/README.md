
# Site24x7

Site24x7 offers unified cloud monitoring for DevOps and IT operations within small to large organizations. The solution monitors the experience of real users accessing websites and applications from desktop and mobile devices. In-depth monitoring capabilities enable DevOps teams to monitor and troubleshoot applications, servers and network infrastructure, including private and public clouds. End-user experience monitoring is done from more than 100 locations across the world and various wireless carriers.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|String|https://www.site24x7.{region}|
|Client ID||True|String||
|Client Secret||True|Password|*****|
|Refresh Token||True|Password|*****|
|Verify SSL||False|Boolean|True|


#### Dependencies
| |
|-|
|python_dateutil-2.9.0.post0-py2.py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|EnvironmentCommon-1.0.0-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|certifi-2026.2.25-py3-none-any.whl|
|idna-3.11-py3-none-any.whl|
|six-1.17.0-py2.py3-none-any.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|


## Actions
#### Ping
Test connectivity to the Site24x7 with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Generate Refresh Token
Generate a refresh token needed for Integration configuration. Please refer to the documentation portal for more details.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Authorization Code|Specify the authorization code.|True|Password|*****|



##### JSON Results
```json
{"refresh_token": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"}
```









## Connectors
#### Site24x7 - Alerts Log Connector
Pull information about alert logs from Site24x7.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Client Secret|Client Secret of the Site24x7 instance.|True|Password|*****|
|DeviceProductField|Enter the source field name in order to retrieve the Product Field name.|True|String|Product Name|
|EventClassId|Enter the source field name in order to retrieve the Event Field name.|True|String|eventType|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|PythonProcessTimeout|Timeout limit for the python process running the current script.|True|Integer|180|
|API Root|API root of the Site24x7 instance. Possible api roots: United States https://www.site24x7.com Europe https://www.site24x7.eu China https://www.site24x7.cn India https://www.site24x7.in Australia https://www.site24x7.net.au|True|String|https://www.site24x7.{region}|
|Refresh Token|Site24x7 Refresh token. You can generate this token using action "Get Refresh Token".|True|Password|*****|
|Client ID|Client ID of the Site24x7 instance.|True|String||
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Site24x7 server is valid.|False|Boolean|true|
|Max Days Backwards|Number of days before the first connector iteration to retrieve alert logs from. This parameter applies to the initial connector iteration after you enable the connector for the first time, or used as a fallback value in cases where connector's last run timestamp expires.|False|Integer|1|
|Max Alert Logs To Fetch|How many alert logs to process per one connector iteration. Default: 100.|False|Integer|10|
|Use whitelist as a blacklist|If enabled, whitelist will be used as a blacklist.|False|Boolean|false|
|Disable Overflow|If enabled, connector will ignore the overflow mechanism.|False|Boolean|true|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




