
# SolarWindsOrion

The Orion Platform offers a single architecture that scales to manage the most complex and geographically dispersed IT environments. SolarWinds scalability engines are designed to provide monitoring and management for large enterprise-class infrastructures. Additional polling engines allow you to scale up to 400,000 elements on a single Orion Platform instance while additional web servers scale the number of supported users. With Enterprise Operations Console (EOC), you can centralize and simplify data management of multiple instances in a single, consolidated view.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|IP Address||True|String|https://x.x.x.x:17778|
|Username||True|String||
|Password||True|Password|*****|
|Verify SSL||False|Boolean|True|


#### Dependencies
| |
|-|
|certifi-2026.4.22-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|idna-3.13-py3-none-any.whl|


## Actions
#### Execute Entity Query
Execute query in SolarWinds Orion based on the IP and Hostname entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Query|Specify the query that needs to be executed. Note: SolarWind queries don’t support “*” notation and you shouldn’t have a WHERE clause in the query, because it is added by the action. Please refer to the action documentation for details.|True|String||
|IP Entity Key|Specify what key should be used with IP entities in the WHERE clause of the query. Please refer to the action documentation for details. Default: IpAddress.|False|String|IpAddress|
|Hostname Entity Key|Specify what key should be used with Hostname entities in the WHERE clause of the query. Please refer to the action documentation for details. Default: Hostname|False|String|Hostname|
|Max Results To Return|Specify how many results should be returned.|False|String|100|



#### Enrich Endpoint
Fetch endpoint's system information by its hostname or IP address.
Timeout - 600 Seconds



#### Execute Query
Execute query in SolarWinds Orion.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Query|Specify the query that needs to be executed. Note: SolarWind queries don’t support “*” notation.|True|String||
|Max Results To Return|Specify how many results should be returned.|False|String|100|



#### Ping
Test connectivity to the SolarWinds Orion with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds









