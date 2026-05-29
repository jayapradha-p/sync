
# McAfeeMvisionEPOV2

McAfee MVISION ePO reduces incident response times, strengthens protection, and simplifies risk and security management using automation and end-to-end security visibility. McAfeeÂ® manages the platform infrastructure, upgrades, and maintenance.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|None|True|URL|https://api.mvision.mcafee.com|
|Client ID|None|True|String||
|Client Secret|None|True|Password|*****|
|API Key|None|True|Password|*****|
|Scopes|None|True|String|epo.device.r epo.device.w epo.evt.r epo.taggroup.r epo.taggroup.w epo.tags.r epo.tags.w mi.user.investigate soc.inv.ade|
|IAM Root|None|False|URL|https://iam.mcafee-cloud.com|
|Verify SSL|None|False|Boolean|True|


#### Dependencies
| |
|-|
|chardet-5.2.0-py3-none-any.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|certifi-2024.7.4-py3-none-any.whl|
|EnvironmentCommon-1.0.0-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|
|idna-3.7-py3-none-any.whl|
|charset_normalizer-3.3.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|
|requests-2.32.3-py3-none-any.whl|


## Actions
#### Add Tag To Device
Add tag to the device in McAfee Mvision ePO V2.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Tag Name|Specify what tag you want to add to endpoint.|True|String||



#### List Devices
List devices that are available in McAfee Mvision ePO V2.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Max Devices to Return|Specify how many devices to return.|False|String|100|



#### List Tags
List tags that are available in McAfee Mvision ePO V2.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Max Tags to Return|Specify how many tags to return.|False|String|100|



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Enrich Endpoint
Fetch device's system information by its hostname or IP address.
Timeout - 600 Seconds



#### Remove Tag From Device
Remove tag from the device in McAfee Mvision ePO V2.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Tag Name|Specify what tag  you want to remove from endpoint.|True|String||









## Connectors
#### McAfee Mvision EPO V2 - Events Connector
Pull events from McAfee Mvision EPO V2.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|API Root of the McAfee Mvision EPO V2 account.|True|String|https://api.mvision.mcafee.com|
|IAM Root|IAM Root of the McAfee Mvision EPO V2 API.|True|String|https://iam.mcafee-cloud.com|
|Client ID|Client ID of the McAfee Mvision EPO V2 account.|True|String||
|Client Secret|Client Secret of the McAfee Mvision EPO V2 account.|True|Password|*****|
|API Key|API Key of the McAfee Mvision EPO V2 account.|True|Password|*****|
|Scopes|Scopes of the McAfee Mvision EPO V2 account.|False|String|epo.device.r epo.device.w epo.evt.r epo.taggroup.r epo.taggroup.w epo.tags.r epo.tags.w mi.user.investigate soc.inv.ade|
|Fetch Max Hours Backwards|Number of hours before the first connector iteration to retrieve alerts from. This parameter applies to the initial connector iteration after you enable the connector for the first time, or used as a fallback value in cases where connector's last run timestamp expires.|False|Int|1|
|Max Alerts To Fetch|How many alerts to process per one connector iteration.|True|Int|50|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the CheckPoint Cloud Guard server is valid.|False|Boolean|true|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




