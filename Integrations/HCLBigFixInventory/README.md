
# HCLBigFixInventory

HCL BigFix Software Inventory provides valuable insight into what the organization owns and what it has installed but does not own along with how often the software is being used.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|API root of the HCL BigFix Inventory instance.|True|String|https://{{ip address}}:9081|
|API Token|API Token of the HCL BigFix Inventory account.|True|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the HCL BigFix Inventory server is valid.|False|Boolean|true|


#### Dependencies
| |
|-|
|certifi-2026.2.25-py3-none-any.whl|
|charset_normalizer-3.4.6-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|idna-3.11-py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|TIPCommon-1.0.11-py2.py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|chardet-7.4.0.post1-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|


## Actions
#### Ping
Test connectivity to the HCL BigFix Inventory with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Enrich Entities
Enrich entities using information from HCL BigFix Inventory. Supported entities: Hostname, IP Address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Custom Fields|Specify a comma-separated list of fields that needs to be returned in addition to the ones that are returned by default.|False|String||
|Create Insight|If enabled, action will create an insight containing all of the retrieved information about the entity.|False|Boolean|true|









