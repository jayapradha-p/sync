
# Intezer

Intezer Integration for Google SecOps SOAR enables security teams to automate the analysis, detection, and response of threats by integrating Intezer's technology into their Google SecOps workflows

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|API root of the Intezer service.|True|String|https://analyze.intezer.com/api/v2-0/|
|API key|Intezer API key|True|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Intezer service is valid.|False|Boolean|true|


#### Dependencies
| |
|-|
|pyasn1_modules-0.4.1-py3-none-any.whl|
|urllib3-2.2.3-py3-none-any.whl|
|cachetools-5.5.0-py3-none-any.whl|
|rsa-4.9-py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|EnvironmentCommon-1.0.2-py2.py3-none-any.whl|
|beautifulsoup4-4.12.3-py3-none-any.whl|
|TIPCommon-1.1.3.2-py2.py3-none-any.whl|
|pyasn1-0.6.1-py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|
|soupsieve-2.6-py3-none-any.whl|
|idna-3.10-py3-none-any.whl|
|certifi-2024.8.30-py3-none-any.whl|
|google_auth-2.35.0-py2.py3-none-any.whl|


## Actions
#### Index File
Index the file's genes into the organizational database.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Index As|Index as trusted or malicious|True|List||
|SHA256|Sha256 to index. Multiple values can be provided as a comma-separated string.|False|String||
|Family Name|Family name to index as|False|String||



#### Get File Report
Get a file analysis report based on an analysis ID or a file hash.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Analysis ID|Specify a comma-separated list of File Analysis IDs to run the action on. Analysis ID is case sensitive. Note: if both "Analysis ID" and "File Hash" are provided, then "File Hash" value will have priority. Multiple values can be provided as a comma-separated string.|False|String|None|
|File Hash|Specify a comma-separated list of file hashes to run the action on. File Hash is case sensitive. Note: if both "Analysis ID" and "File Hash" are provided, then "File Hash" value will have priority. Multiple values can be provided as a comma-separated string.|False|String|None|
|Private Only|Whether to show only private reports (relevant only for hashes).|False|Boolean|false|
|Wait For Completion|Whether to wait for the analysis to complete before returning the report.|False|Boolean|false|



#### Detonate Hash
Analyze a file hash (SHA1, SHA256, or MD5) on Intezer Analyze.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File Hash|Hash of the desired report. Multiple values can be provided as a comma-separated string.|False|String||



#### Detonate URL
Analyze a suspicious URL with Intezer.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Url|URL to analyze. Multiple values can be provided as a comma-separated string.|False|String||



#### Ping
Test connectivity to the Intezer with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Submit File
Submit a file for analysis.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File Paths|The paths of the file to analyze.|True|String|None|



#### Get Alert
Get an ingested alert triage and response information using alert ID.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Alert ID|The alert id to query.|True|String||
|Wait For Completion|Whether to wait for the analysis to finish.|False|Boolean|false|



#### Get URL Report
Get a URL analysis report based on a URL analysis ID.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Analysis ID|Specify a comma-separated list of URL Analysis IDs to run the action on. Analysis ID is case sensitive. The analysis ID is returned when submitting a URL for analysis. Multiple values can be provided as a comma-separated string.|True|String||
|Wait For Completion|Whether to wait for the analysis to finish.|False|Boolean|false|



#### Unset Index File
Unset file's indexing.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|SHA256|SHA256 file to unset the indexing. Multiple values can be provided as a comma-separated string.|False|String||



#### Submit Alert
Submit a new alert including the raw alert information to Intezer for processing.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Source|The source of the alert|True|String||
|Raw Alert|Alert raw data in JSON format|True|String||
|Alert Mapping|Mapping to use for the alert in JSON format|True|String||



#### Submit Suspicious Email
Submit a suspicious phishing email in a raw format (.MSG or .EML) to Intezer for processing
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Email File Path|Path to the email file|True|String|None|



#### Detonate File
Analyze a file from Splunk vault with Intezer.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File Path|Path to file for analyzing. Multiple values can be provided as a comma-separated string.|True|String||
|Related Alert ID|The alert id related to the file.|False|String||



#### Submit Hash
Submit a hash for analysis.
Timeout - 600 Seconds









