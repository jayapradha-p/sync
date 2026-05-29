
# RemoteAgentUtilities

Remote Agents Utilities enable file transfers between a Google SecOps machine to a machine which has a remote agent installed on it and vice versa.

Python Version - 3


#### Dependencies
| |
|-|
|certifi-2026.4.22-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|requests-2.33.1-py3-none-any.whl|
|TIPCommon-1.0.11-py2.py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|idna-3.13-py3-none-any.whl|


## Actions
#### Deserialize A File
Deserialize a file from a base64 string and save it to disk.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File Name|File Name. The purpose is to get as a placeholder from prev action (key in json result - file_name)|True|String||
|File base64|File base64. The purpose is to get as a placeholder from prev action (key in json result - base64_file_content)|True|String||



#### Serialize A File
Serialize a file to a base64 string.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File Path|Full path of the file|True|String||



##### JSON Results
```json
{"file_name": "example.txt", "base64_file_content": "SGVsbG8gV29ybGQ="}
```



#### Ping
Test Connectivity
Timeout - 600 Seconds









