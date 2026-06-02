
# CheckPointSandBlast

Protect your organization from zero-day cyber attacks with SandBlast Network, the marketâ€™s leading advanced network threat prevention solution. Increase productivity while creating a secure environment with innovative technologies like threat emulation, threat extraction and artificial intelligence.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|String|https://<service_address>/tecloud/api/<version>/file|
|API Key||True|Password|*****|
|Verify SSL||False|Boolean||


#### Dependencies
| |
|-|
|requests-2.32.4-py3-none-any.whl|
|idna-3.13-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|certifi-2026.4.22-py3-none-any.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|


## Actions
#### Ping
Test connectivity to the Check Point SandBlast with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Query
Get threat reputation information about FILEHASH entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Threshold|Mark entity as suspicious if severity is equal or above the given threshold.|True|String|0|



#### Upload File
Upload files for analysis
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File Path|The full path of the file to upload. For multiple, use comma separated values.|True|String||
|Enable Threat Emulation feature|If enabled, threat emulation feature will be enabled for the upload. By default, if no features are selected, threat emulation will be used.|False|Boolean||
|Enable AntiVirus feature|If enabled, antivirus feature will be enabled for the upload. By default, if no features are selected, threat emulation will be used.|False|Boolean||
|Enable Threat Extraction feature|If enabled, threat extraction feature will be enabled for the upload. By default, if no features are selected, threat emulation will be used.|False|Boolean||









