
# Splash

Splash is a javascript rendering service with an HTTP API. It's a lightweight browser with an HTTP API, implemented in Python 3 using Twisted and QT5. It's fast, lightweight and state-less which makes it easy to distribute.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|String|https://{{ip address}}:8050|
|Verify SSL||False|Boolean|True|


#### Dependencies
| |
|-|
|certifi-2026.2.25-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|idna-3.11-py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|


## Actions
#### Enrich Entities
Enrich entities using information from Splash. Supported entities: URL, IP Address. Note: URLs need to have a schema. For IP addresses, action will add the “HTTPS” schema.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Create Insight|If enabled, action will create an insight containing all of the retrieved information about the entity.|False|Boolean|true|
|Include PNG Screenshot|If enabled, action will return a PNG screenshot in an insight. Note: “Create Insight” should be enabled for this parameter to work.|False|Boolean|true|
|Include History|If enabled, action will return history information.|False|Boolean|false|
|Include HAR|If enabled, action will return HAR information.|False|Boolean|false|



#### Ping
Test connectivity to the Splash with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds









