
# AnyRun

Interactive online malware analysis service for dynamic and static research of most types of threats using any environments.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Key|None|True|Password|*****|


#### Dependencies
| |
|-|
|charset_normalizer-3.3.2-py3-none-any.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|
|chardet-5.2.0-py3-none-any.whl|
|idna-3.8-py3-none-any.whl|
|certifi-2024.8.30-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|


## Actions
#### Ping
Test Connectivity
Timeout - 600 Seconds



#### AnalyzeURL
Create Any.Run analysis task for the provided URL. Note: URL can be provided either as a Siemplify URL entity (artifact) or as an action input parameter. If the URL is provided both as an entity and input parameter - action will be executed on the input parameter.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|URL For Analysis|Specify URL to analyze. If URL is provided in both as entity and as this input parameter - action will be executed on input parameter.|True|String||
|Wait for the report?|Specify whether action should wait for the report creation. Report also can be obtained later with Get report action once scan is completed.|False|Boolean|True|
|Try to create submission for x times|How many attempts action should make to check if the API concurrency limit is not exceeded and try to create a new submission. Check is made every 2 seconds.|True|String|30|
|OS Version|OS version to run analysis on.|False|List|7|
|Operation System Bitness|Bitness of Operation System|False|List|32|
|OS Environment Type|Environment type to run analysis on.|False|List|complete|
|Network Connection Status|Network connection state for analysis.|False|List|On|
|FakeNet Feature Status|FakeNet feature state for analysis.|False|List|false|
|Use TOR|Use TOR or not while running analysis.|False|List|false|
|opt_network_mitm|HTTPS MITM proxy option.|False|List|false|
|opt_network_geo|Geo location option.|False|List|fastest|
|opt_kernel_heavyevasion|Heavy evasion option.|False|List|false|
|opt_privacy_type|Privacy settings for analysis.|False|List|By Link|
|obj_ext_startfolder|Start location for analysis.|False|List|temp|
|opt_timeout|Timeout period for analysis in range from 10 to 9999 seconds.|False|String|60|



#### AnalyzeFileURL
Create Any.Run file analysis task. Note: Action is not working with Siemplify entities, URL to file to analyze should be provided as action input parameter.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|URL to File|Specify URL to file to download and analyze.|True|String||
|Wait for the report?|Specify whether action should wait for the report creation. Report also can be obtained later with Get report action once scan is completed.|False|Boolean|True|
|Try to create submission for x times|How many attempts action should make to check if the API concurrency limit is not exceeded and try to create a new submission. Check is made every 2 seconds.|True|String|30|
|OS Version|OS version to run analysis on.|False|List|7|
|Operation System Bitness|Bitness of Operation System|False|List|32|
|OS Environment Type|Environment type to run analysis on.|False|List|complete|
|Network Connection Status|Network connection state for analysis.|False|List|On|
|FakeNet Feature Status|FakeNet feature state for analysis.|False|List|false|
|Use TOR|Use TOR or not while running analysis.|False|List|false|
|opt_network_mitm|HTTPS MITM proxy option.|False|List|false|
|opt_network_geo|Geo location option.|False|List|fastest|
|opt_kernel_heavyevasion|Heavy evasion option.|False|List|false|
|opt_privacy_type|Privacy settings for analysis.|False|List|By Link|
|obj_ext_startfolder|Start location for analysis.|False|List|temp|
|opt_timeout|Timeout period for analysis in range from 10 to 9999 seconds.|False|String|60|



#### Search Report History
Search Any.Run scans history. Note: Action is not working with Siemplify entities, only action input parameters are used.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Submission Name|Specific submission name to search for.|False|String||
|Search in last x scans|Search for report in last x analyses executed in Any.Run.|True|String|25|
|Skip first x scans|Skip first x scans returned by Any.Run API.|False|String|0|
|Get team history?|Specify whether to get team history or not.|False|Boolean|false|



#### AnalyzeFile
Create Any.Run file analysis task. Note: Action is not working with Siemplify entities, full path to file to analyze should be provided as action input parameter.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File Path|Specify full path to file to analyze.|True|String||
|Wait for the report?|Specify whether action should wait for the report creation. Report also can be obtained later with Get report action once scan is completed.|False|Boolean|True|
|Try to create submission for x times|How many attempts action should make to check if the API concurrency limit is not exceeded and try to create a new submission. Check is made every 2 seconds.|True|String|30|
|OS Version|OS version to run analysis on.|False|List|7|
|Operation System Bitness|Bitness of Operation System|False|List|32|
|OS Environment Type|Environment type to run analysis on.|False|List|complete|
|Network Connection Status|Network connection state for analysis.|False|List|On|
|FakeNet Feature Status|FakeNet feature state for analysis.|False|List|false|
|Use TOR|Use TOR or not while running analysis.|False|List|false|
|opt_network_mitm|HTTPS MITM proxy option.|False|List|false|
|opt_network_geo|Geo location option.|False|List|fastest|
|opt_kernel_heavyevasion|Heavy evasion option.|False|List|false|
|opt_privacy_type|Privacy settings for analysis.|False|List|By Link|
|obj_ext_startfolder|Start location for analysis.|False|List|temp|
|opt_timeout|Timeout period for analysis in range from 10 to 9999 seconds.|False|String|60|



#### Get Report
Get Any.Run report from previous analysis based on the provided Siemplify FileHash, Filename or URL entity. Note: Action supports filehash entity in md-5, sha-1 and sha-256 formats.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Threshold|Mark entity as suspicious if the score value for the entity is above the specified threshold.|True|String|0|
|Search in last x scans|Search for report in last x analysises executed in Any.Run.|True|String|25|
|Create Insight?|Specify whether to create insight based on the report data.|False|Boolean|false|
|Fetch latest report?|Specify whether to return latest analysis report or all found reports for the provided entity.|False|Boolean|true|









