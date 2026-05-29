
# ForeScoutCounterACT

The Forescout device visibility platform provides insight into the diverse types of devices connected to your heterogeneous network—from campus and data center to cloud and operational technology networks. In other words, your extended enterprise. With one platform, you gain a consolidated view of traditional systems, mobile and IoT devices, virtual machines and cloud instances, and now, operational technology (OT) systems.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|String|https://{ip address}|
|Username||True|String||
|Password||True|Password|*****|
|CA Certificate File||False|String||
|Verify SSL||False|Boolean|true|


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
#### Enrich Entities
Enrich entities using information from ForeScout CounterACT. Supported entities: IP, Mac Address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Create Insight|If enabled, action will create insights containing enrichment information.|False|Boolean|True|



#### Ping
Test connectivity to the ForeScout CounterACT with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds









