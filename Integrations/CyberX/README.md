
# CyberX

The most widely-deployed ICS, SCADA & IIoT security platform that continuously reduces OT network risk via ICS threat monitoring & asset discovery.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|URL||
|Access Token||True|String||
|Verify SSL||False|Boolean||


#### Dependencies
| |
|-|
|urllib3-2.6.3-py3-none-any.whl|
|charset_normalizer-3.4.6-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|idna-3.11-py3-none-any.whl|
|requests-2.32.5-py3-none-any.whl|
|certifi-2026.2.25-py3-none-any.whl|


## Actions
#### Get Alerts
 Fetch list of all alerts detected by XSense.
Timeout - 600 Seconds



#### Ping
Test CyberX connectivity.
Timeout - 600 Seconds



#### Get Events
Fetch list of events reported to the event log.
Timeout - 600 Seconds



#### Get Device Vulnerability Report
Fetch vulnerability report for each endpoint.
Timeout - 600 Seconds



#### Get Connections for Endpoint
Get list of connections for each device.
Timeout - 600 Seconds



#### Enrich Endpoints
Fetch endpoint information.
Timeout - 600 Seconds









