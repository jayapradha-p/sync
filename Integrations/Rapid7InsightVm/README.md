
# Rapid7InsightVm

InsightVM vulnerability management software monitors exposures in real-time and adapts to new threats with fresh data, ensuring you can always act at the moment of impact.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root||True|String|https://<host>:<port>/api/3|
|Username||True|String||
|Password||True|Password|*****|
|Verify SSL||False|Boolean|False|


#### Dependencies
| |
|-|
|certifi-2026.4.22-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|arrow-1.4.0-py3-none-any.whl|
|tzdata-2026.2-py2.py3-none-any.whl|
|EnvironmentCommon-1.0.1-py2.py3-none-any.whl|
|python_dateutil-2.9.0.post0-py2.py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|TIPCommon-1.0.12-py2.py3-none-any.whl|
|idna-3.13-py3-none-any.whl|
|six-1.17.0-py2.py3-none-any.whl|


## Actions
#### Enrich Asset
Enrich an asset.
Timeout - 600 Seconds



##### JSON Results
```json
[{"EntityResult": {"users": [{"fullName": "XXX", "id": "XX", "name": "XXX"}], "rawRiskScore": "XXXXXX", "userGroups": [{"id": "XXX", "name": "XX"}], "osFingerprint": {"product": "XXXX", "vendor": "XXXXX", "description": "XXXXXXXXXXXX", "family": "XXXXX", "version": "XXXXXX", "systemName": "XXXXXXXXXX", "architecture": "XXXX", "id": "XX"}, "addresses": [{"ip": "XXXXX", "mac": "XXXXX"}], "links": [{"href": "XXXXXX", "rel": "XXXX"}], "assessedForPolicies": "XXXXX", "ip": "XXX.XX.XX.XX", "hostName": "XXXXXX.XXXXXX", "ids": [{"source": "XXXXX", "id": "XXXXX-XXXXX-XXXX-XXXX-XXXXX"}], "riskScore": "XXXXXXXX", "mac": "XX", "hostNames": [{"source": "XXXX", "name": "XXXXX.XXXXX"}], "vulnerabilities": {"moderate": "XX", "exploits": "XX", "malwareKits": "XXX", "severe": "XXX", "critical": "XX", "total": "XX"}, "type": "XXXX", "services": [{"product": "XXXX", "protocol": "XXXX", "name": "XXXX", "links": [{"href": "XXXXX", "rel": "XXXX"}], "version": "XXX", "family": "XXX", "vendor": "XXXX", "port": "XX", "configurations": [{"name": "XXXX", "value": "XXXX"}]}], "assessedForVulnerabilities": "XXXX", "software": [{"product": "XXXX", "version": "XXXXXX", "vendor": "XXXX", "description": "XXXXXXXXXXXX", "id": "XX"}], "os": "XXXXXXXXXXXXXXX", "id": 8, "history": [{"date": "2021-07-06T15:30:20.787Z", "scanId": 1, "version": 1, "type": "XXXX"}]}, "Entity": "XXX.XX.XXX.XX"}]
```



#### Launch Scan
Start a scan for a specific site.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Scan Engine|The name of the engine to use in the scan.|True|String||
|Scan Name|The scan name.|False|String||
|Scan Template|The name of the template to use in the scan.|True|String||
|Site Name|The name of the site to run the scan on.|True|String||
|Fetch Results|Whether to wait for the scan to complete and get its results or not.|False|Boolean||



##### JSON Results
```json
{"status": "finished", "scanType": "Manual", "assets": 1, "links": [{"href": "https://1.1.1.1:3780/api/3/scans/8", "rel": "self"}], "vulnerabilities": {"severe": 12, "total": 18, "critical": 0, "moderate": 6}, "startTime": "2019-04-11T07:44:00.095Z", "duration": "PT7M58.298S", "engineName": "Local scan engine", "endTime": "2019-04-11T07:51:58.393Z", "id": 8, "scanName": "siemplify_20190411-104353"}
```



#### Get Scan Results
Get scan results by ID
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Scan ID|The ID of the scan.|True|String|None|



##### JSON Results
```json
{"STATUS": {"STATE": "Finished"}, "EXPIRATION_DATETIME": "2019-02-04T13:11:15Z", "TITLE": "Scan scan/1533110666.07264 Report", "USER_LOGIN": "login-example", "OUTPUT_FORMAT": "PDF", "LAUNCH_DATETIME": "2019-01-28T13:11:14Z", "TYPE": "Scan", "ID": "775111", "SIZE": "22.17 KB"}
```



#### List Scans
List scans
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Days Backwards|Number of days backwards to fetch scans from.|True|String||



##### JSON Results
```json
[{"status": "finished", "scanType": "Manual", "assets": 1, "links": [{"href": "https://1.1.1.1:3780/api/3/scans/8", "rel": "self"}], "vulnerabilities": {"severe": 12, "total": 18, "critical": 0, "moderate": 6}, "startTime": "2019-04-11T07:44:00.095Z", "duration": "PT7M58.298S", "engineName": "Local scan engine", "endTime": "2019-04-11T07:51:58.393Z", "id": 8, "scanName": "siemplify_20190411-104353"}]
```



#### Ping
Test Connectivity
Timeout - 600 Seconds









## Connectors
#### Rapid7 InsightVm - Vulnerabilities Connector
Pull information about asset vulnerabilities from Rapid7 InsightVm. Note: whitelist filter works with "protocol" parameter.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|DeviceProductField|Enter the source field name in order to retrieve the Product Field name.|True|String|Product Name|
|EventClassId|Enter the source field name in order to retrieve the Event Field name.|True|String|type|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|PythonProcessTimeout|Timeout limit for the python process running the current script.|True|Integer|500|
|API Root|API root of the Rapid7 InsightVm instance.|True|String|https://{ip}:3780|
|Username|Username of the Rapid7 InsightVm account.|True|String||
|Password|Password of the Rapid7 InsightVm account.|True|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Rapid7 InsightVm server is valid.|False|Boolean|true|
|Lowest Severity To Fetch|Lowest Severity that needs to be used to fetch vulnerabilities. Possible values: Moderate, Severe, Critical. If nothing is provided, the connector will fetch vulnerabilities with all severities.|False|String|Moderate|
|Max Assets To Process|Amount of assets that need to be processed per 1 connector iteration. Note: it’s not recommended to increase the value of this parameter, because the connector will be more prone to timeouts.|False|Integer|5|
|Grouping Mechanism|Grouping mechanism that will be used to create Siemplify Alerts. Possible values: Host, None. If Host is provided, the connector will create 1 Siemplify Alert containing all of the vulnerabilities related to the host. If None or invalid value is provided, the connector will create a new Siemplify Alert for each separate vulnerability per host.|True|String|Host|
|Use whitelist as a blacklist|If enabled, whitelist will be used as a blacklist.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




