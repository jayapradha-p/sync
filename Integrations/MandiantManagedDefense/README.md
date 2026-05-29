
# MandiantManagedDefense

Mandiant Managed Defense provides 24/7 managed detection and response (MDR) with access to frontline experts who monitor your security technology to help find and investigate threats, proactively hunt for ongoing or past breaches, and respond before attacks impact your business.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|API root of the Mandiant instance.|True|String|https://api.services.mandiant.com|
|Client ID|Client ID of the Mandiant Managed Defense account.|True|String||
|Client Secret|Client Secret of the Mandiant Managed Defense account.|True|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Mandiant server is valid.|False|Boolean|true|


#### Dependencies
| |
|-|
|beautifulsoup4-4.12.3-py3-none-any.whl|
|cachetools-5.5.0-py3-none-any.whl|
|pyasn1-0.6.0-py2.py3-none-any.whl|
|rsa-4.9-py3-none-any.whl|
|google_auth_httplib2-0.2.0-py2.py3-none-any.whl|
|googleapis_common_protos-1.64.0-py2.py3-none-any.whl|
|httplib2-0.22.0-py3-none-any.whl|
|google_api_python_client-2.142.0-py2.py3-none-any.whl|
|pyparsing-3.1.4-py3-none-any.whl|
|google_auth-2.34.0-py2.py3-none-any.whl|
|google_api_core-2.19.1-py3-none-any.whl|
|httpcore-1.0.5-py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|EnvironmentCommon-1.0.2-py2.py3-none-any.whl|
|certifi-2024.7.4-py3-none-any.whl|
|idna-3.8-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|
|anyio-4.4.0-py3-none-any.whl|
|h11-0.14.0-py3-none-any.whl|
|proto_plus-1.24.0-py3-none-any.whl|
|uritemplate-4.1.1-py2.py3-none-any.whl|
|httpx-0.27.0-py3-none-any.whl|
|pyasn1_modules-0.4.0-py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|
|pycryptodome-3.20.0-cp35-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|
|TIPCommon-1.1.9.0-py2.py3-none-any.whl|
|sniffio-1.3.1-py3-none-any.whl|
|soupsieve-2.6-py3-none-any.whl|
|protobuf-5.27.3-cp38-abi3-manylinux2014_x86_64.whl|


## Actions
#### Ping
Test connectivity to the Mandiant MD with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds









## Connectors
#### Mandiant Managed Defense - Investigations Connector
Pull investigation from Mandiant Managed Defense. Dynamic List works with the "name" parameter.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|DeviceProductField|Enter the source field name in order to retrieve the Product Field name.|True|String|Product Name|
|EventClassId|Enter the source field name in order to retrieve the Event Field name.|True|String|type|
|PythonProcessTimeout|Timeout limit for the python process running the current script.|True|Integer|180|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|API Root|API root of the Mandiant instance.|True|String|https://api.services.mandiant.com|
|Client ID|Client ID of the Mandiant Managed Defense account.|True|String||
|Client Secret|Client Secret of the Mandiant Managed Defense account.|True|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Mandiant server is valid.|False|Boolean|true|
|Status Filter|Status filter for the investigations. Note: If nothing is provided, investigations with all status will be ingested. Possible Values:open, resolved, disputed, false-positive|False|String|open,resolved,disputed,false-positive|
|Max Hours Backwards|Number of hours before the first connector iteration to retrieve alerts from. This parameter applies to the initial connector iteration after you enable the connector for the first time, or used as a fallback value in cases where connector's last run timestamp expires.|True|Integer|24|
|Padding Time|The padding period in hours to fetch investigations. Represents hours. The maximum value is 12 hours.|False|Integer|12|
|Max Investigations To Fetch|How many investigations to process per one connector iteration. Maximum: 100|True|Integer|100|
|Use dynamic list as a blocklist|If enabled, the dynamic list will be used as a blocklist.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




