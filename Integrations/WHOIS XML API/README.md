
# WHOIS XML API

Whois API provides consistent, well-structured whois data in XML & JSON. It provides WHOIS record and domain related information. 

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Key|API Key|True|Password|*****|


#### Dependencies
| |
|-|
|certifi-2025.6.15-py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|idna-3.10-py3-none-any.whl|
|urllib3-2.5.0-py3-none-any.whl|
|charset_normalizer-3.4.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|


## Actions
#### Enrich Entities
Adds Enrichment data extracted from whois XML API product and presents it in the Entity Explorer
Timeout - 600 Seconds



#### Get Domain Details
Get the domain details and present them as a Json result 
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Domain Name|The domain to scan|True|String|google.com|
|Check availability|Check availability|False|Boolean|false|



#### Ping
Check connectivity
Timeout - 600 Seconds









