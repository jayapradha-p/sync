
# McAfeeTIEDXL

McAfee Threat Intelligence Exchange optimizes threat detection and response by closing the gap from malware encounter to containment from days, weeks, and months down to milliseconds.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Server Address||True|IP_OR_HOST|ssl://{IP}:{PORT}|
|Broker CA Bundle Path||True|String||
|Client Cert File Path||True|String||
|Client Key File Path||True|String||


#### Dependencies
| |
|-|
|configobj-5.0.9-py2.py3-none-any.whl|
|certifi-2026.4.22-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|dxltieclient-0.3.0-py2.py3-none-any.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|oscrypto-1.3.0-py2.py3-none-any.whl|
|dxlbootstrap-0.2.2-py2.py3-none-any.whl|
|msgpack-1.1.2-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|PySocks-1.7.1-py3-none-any.whl|
|types_python_dateutil-2.9.0.20260408-py3-none-any.whl|
|python_dateutil-2.9.0.post0-py2.py3-none-any.whl|
|requests-2.33.1-py3-none-any.whl|
|dxlclient-5.6.0.0-py2.py3-none-any.whl|
|TIPCommon-1.0.11-py2.py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|idna-3.13-py3-none-any.whl|
|arrow-1.3.0-py3-none-any.whl|
|asn1crypto-1.5.1-py2.py3-none-any.whl|
|six-1.17.0-py2.py3-none-any.whl|


## Actions
#### Ping
Test connectivity
Timeout - 600 Seconds



#### Get File Reputation
Get file reputation
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Enrich with all services|If checked, enrich with all results from all returned services. Else, store only the worst reputation as enrichment.|False|Boolean|False|



#### Get File References
Get references for a file (the agent on which the file was used)
Timeout - 600 Seconds



#### Set File Reputation
Set a file's enterprise reputation
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Trust Level|The trust level to set to the file's reputation|True|String||
|File Name|The name of the file|False|String|None|
|Comment|The comment to add to the file's reputation|False|String|None|









