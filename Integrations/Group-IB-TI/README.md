
# Group-IB-TI

This integration connects Group-IB Threat Intelligence (GIB TI) with the Google Chronicle platform. It automatically ingests threat feeds from GIB TI and transforms them into  Chronicle alerts, populated with corresponding entities. In case of any queries, please reach out to integartion@group-ib.com.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Verify SSL|Verify the server's SSL certificate|False|Boolean|true|
|API login|The email used to login to Group-IB TI |True|Email|None|
|API key|API token generated in your Group-IB TI profile |True|Password|*****|
|API URL|Base URL for Group-IB TI API |True|String|https://tap.group-ib.com/api/v2/|


#### Dependencies
| |
|-|
|PyYAML-6.0.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|
|httplib2-0.30.0-py3-none-any.whl|
|urllib3-2.5.0-py3-none-any.whl|
|google_auth_httplib2-0.2.0-py2.py3-none-any.whl|
|cyberintegrations-0.11.1-py3-none-any.whl|
|cachetools-5.5.2-py3-none-any.whl|
|pyparsing-3.2.3-py3-none-any.whl|
|httpx-0.28.1-py3-none-any.whl|
|httpcore-1.0.9-py3-none-any.whl|
|uritemplate-4.2.0-py3-none-any.whl|
|certifi-2025.8.3-py3-none-any.whl|
|rsa-4.9.1-py3-none-any.whl|
|h11-0.16.0-py3-none-any.whl|
|requests-2.32.5-py3-none-any.whl|
|TIPCommon-2.2.10-py2.py3-none-any.whl|
|pyaml-23.5.8-py3-none-any.whl|
|anyio-4.10.0-py3-none-any.whl|
|EnvironmentCommon-1.0.2-py2.py3-none-any.whl|
|pyasn1_modules-0.4.2-py3-none-any.whl|
|charset_normalizer-3.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|protobuf-6.32.0-py3-none-any.whl|
|pyasn1-0.6.1-py3-none-any.whl|
|idna-3.10-py3-none-any.whl|
|sniffio-1.3.1-py3-none-any.whl|
|googleapis_common_protos-1.70.0-py3-none-any.whl|
|typing_extensions-4.15.0-py3-none-any.whl|
|google_api_core-2.25.1-py3-none-any.whl|
|pycryptodome-3.23.0-cp37-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|
|proto_plus-1.26.1-py3-none-any.whl|
|google_auth-2.40.3-py2.py3-none-any.whl|
|google_api_python_client-2.179.0-py3-none-any.whl|
|validators-0.35.0-py3-none-any.whl|


## Actions
#### Get-TI-Search-Info
Search Domain, IP Address, File Hash, Bank Card, Email in Group-IB TI database.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Enable mapping parser|Enable or Disable mapping parser before return JSON output|False|Boolean|false|



#### Get-Graph-Info
Used to get WHOIS information based on Domain or IP Address.
Timeout - 600 Seconds



#### Get-Collection-Info-Async
Help to extract data from Group-IB TI database by chosen collection. Can be used to run daily to get fresh updates only. This Action ignore any entities. Use the input entity as the start trigger.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Enable mapping parser|Enable or Disable mapping parser before return JSON output|False|Boolean|false|
|Collection|Choose required collection to download|True|List|apt/threat|
|Start date|Set start date to download collection data. Date format YYYY-MM-DD (2023-09-01).|False|String|None|
|Portion limit|Each Action run return response from TI Portal API, which contains portions. This parameter let you control the number of received portions.|True|List|100|



#### Ping
Ping to test Group-IB Threat Intelligence connection. Also gives JSON output of available collections, based on subscription.
Timeout - 600 Seconds



#### Get-TI-Search-Info-By-Collection
Search Domain, IP Address, URL, File Hash, Bank Card, Email in Group-IB TI database. Specify tag to get targeted field results.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Enable mapping parser|Enable or Disable mapping parser before return JSON output|False|Boolean|false|
|Collection|Choose required collection to download|True|List|apt/threat|
|Search tag|By default Tag is empty:  q=<Serach Parameter> (q=8.8.8.8). If Tag is set to "domain":  q=<Tag>:<Search Parameter> (q=domain:google.com).|False|String||









## Connectors
#### TI IoC Hash Connector
TI Scheduled Connector to retrieve IoCs - Hash.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API key|API key - API key, generated at your Group-IB TI Profile|True|Password|*****|
|API login|API login - your email address used to enter the Group-IB TI Portal|True|Email|example@group-ib.com|
|API URL|API URL - Group-IB TI Portal URL|True|String|https://tap.group-ib.com/api/v2/|
|Case name|Case name to display|True|String|IoC Hash|
|Case severity|Type one of the following:Informative,Low,Medium,High,Critical|True|String|Critical|
|Case type|Case type to trigger an Action|True|String|IoC|
|Start date|Set start date to download collection data. Date format YYYY-MM-DD (2023-09-01). If None - one day back is set by default.|False|String||
|Verify SSL|Whether to verify SSL certificates|False|Boolean|true|


#### TI IoC IP Connector
TI Scheduled Connector to retrieve IoCs - IP.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API login|API login - your email address used to enter the Group-IB TI Portal|True|Email|example@group-ib.com|
|API URL|API URL - Group-IB TI Portal URL|True|String|https://tap.group-ib.com/api/v2/|
|Case name|Case name to display|True|String|IoC IP|
|Case severity|Type one of the following:Informative,Low,Medium,High,Critical|True|String|Critical|
|Case type|Case type to trigger an Action|True|String|IoC|
|Start date|Set start date to download collection data. Date format YYYY-MM-DD (2023-09-01). If None - one day back is set by default.|False|String||
|API key|API key - API key, generated at your Group-IB TI Profile|True|Password|*****|
|Verify SSL|Whether to verify SSL certificates|False|Boolean|true|




