
# APIVoid

Database of API services mostly focused on threat analysis and threat intelligence, that can be easily integrated anywhere.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root||True|String|https://endpoint.apivoid.com|
|Api Key||True|Password|*****|
|Verify SSL||False|Boolean|False|


#### Dependencies
| |
|-|
|requests-2.32.4-py3-none-any.whl|
|TIPCommon-1.0.11-py2.py3-none-any.whl|
|idna-3.13-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|certifi-2026.4.22-py3-none-any.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|


## Actions
#### Get URL Reputation
Get safety reputation and risk score of an URL
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Threshold|URL risk threshold. The threshold must be a numeric value. e.g. 3|True|String||



#### Get Ip Reputation
Detect potentially malicious IP addresses commonly used for spam, to attack websites or to commit fraudulent activities
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Threshold|IP risk threshold. The threshold must be a numeric value. e.g. 3|True|String||
|Create Insights|Specify whether the action should create insights or not.|False|Boolean|true|



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Get Screenshot
Capture a high-quality screenshot of any website or URL
Timeout - 600 Seconds



#### Get domain reputation
Check if a domain is blacklisted by popular and trusted domain blacklist services.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Threshold|Domain risk threshold. The threshold must be a numeric value. e.g. 3|True|String||
|Create Insights|Specify whether the action should create insights or not.|False|Boolean|true|



#### Verify Email
Check if an email is disposable, if it has MX records and more
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Threshold|Email risk threshold. The threshold must be a numeric value. e.g. 3|True|String||









