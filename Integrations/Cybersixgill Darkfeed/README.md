
# Cybersixgill Darkfeed

Powered by the broadest, automated collection from the deep and dark web, Cybersixgill Darkfeed is a feed of malicious indicators of compromise (IOCs), including domains, URLs, hashes and IP addresses. IOCs are automatically extracted and delivered in real-time, and it is actionable, allowing Google SecOps customers to receive and preemptively block items that threaten their organization.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Client Id|Client Id|True|String|Client_id|
|Client Secret|Secret Key|True|Password|*****|


#### Dependencies
| |
|-|
|certifi-2025.6.15-py3-none-any.whl|
|sixgill_clients-0.2.26-py2.py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|idna-3.10-py3-none-any.whl|
|urllib3-2.5.0-py3-none-any.whl|
|charset_normalizer-3.4.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|


## Actions
#### Ping

Timeout - 600 Seconds



##### JSON Results
```json
{}
```









## Connectors
#### Cybersixgill - Darkfeed Connector
Powered by the broadest, automated collection from the deep and dark web, Cybersixgill Darkfeed is a feed of malicious indicators of compromise (IOCs), including domains, URLs, hashes and IP addresses. IOCs are automatically extracted and delivered in real-time, and it is actionable, allowing Siemplify customers to receive and preemptively block items that threaten their organization.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|PythonProcessTimeout|The timeout limit (in seconds) for the python process running current script|True|String|30|
|EventClassId|The field name used to determine the event name (sub-type)|True|String|Cybersixgill Darkfeed |
|DeviceProductField|The field name used to determine the device product|True|String|Cybersixgill Darkfeed |
|Client Secret|Secret Key|True|Password|*****|
|Client Id|Client ID|True|String|Client_Id|
|Alerts Limit|Number of alerts to be ingested into the platform|True|Integer|20|




