
# TrendMicroDDAN

Deep Discovery Analyzer extends the value of existing security investments from Trend Micro and third-parties (through a web services API) by providing custom sandboxing and advanced analysis.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|API root of the Trend Micro DDAN instance.|True|String|https://{ip address}|
|API Key|API key of the Trend Micro DDAN instance.|True|Password|*****|
|Verify SSL|If enabled, verifies that the SSL certificate for the connection to the Trend Micro DDAN is valid.|False|Boolean|true|


#### Dependencies
| |
|-|
|charset_normalizer-3.3.2-py3-none-any.whl|
|TIPCommon-1.0.12-py2.py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|
|chardet-5.2.0-py3-none-any.whl|
|xmltodict-0.13.0-py2.py3-none-any.whl|
|certifi-2024.7.4-py3-none-any.whl|
|idna-3.8-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|


## Actions
#### Ping
Test connectivity to Trend Micro DDAN with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Submit File
Submit files in Trend Micro DDAN. Note: Action is running as async, adjust the script timeout value in Chronicle SOAR IDE for action as needed.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File Paths|Specify a comma-separated list of the absolute file paths that point to the file that needs to be analyzed.|True|String||
|Fetch Event Log|If enabled, action will fetch event logs related to the files.|False|Boolean|true|
|Fetch Suspicious Objects|If enabled, action will fetch suspicious objects.|False|Boolean|true|
|Fetch Sandbox Screenshot|If enabled, action will try to fetch a sandbox screenshot related to the files.|False|Boolean|false|
|Resubmit File|If enabled, action will not check if there was a submission for this file previously.|False|Boolean|true|
|Max Event Logs To Return|Specify how many event logs to return. Default: 50. Max: 200.|False|String|50|
|Max Suspicious Objects To Return|Specify how many suspicious objects to return. Default: 50. Max: 200.|False|String|50|



#### Submit File URL
Submit a file via URLs in Trend Micro DDAN. Note: Action is running as async, adjust the script timeout value in Chronicle SOAR IDE for action as needed.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File URLs|Specify a comma-separated list of the URLs that point to the file that needs to be analyzed.|True|String||
|Fetch Event Log|If enabled, action will fetch event logs related to the files.|False|Boolean|true|
|Fetch Suspicious Objects|If enabled, action will fetch suspicious objects.|False|Boolean|true|
|Fetch Sandbox Screenshot|If enabled, action will try to fetch a sandbox screenshot related to the files.|False|Boolean|false|
|Resubmit File|If enabled, action will not check if there was a submission for this file previously.|False|Boolean|true|
|Max Event Logs To Return|Specify how many event logs to return. Default: 50. Max: 200.|False|String|50|
|Max Suspicious Objects To Return|Specify how many suspicious objects to return. Default: 50. Max: 200.|False|String|50|









