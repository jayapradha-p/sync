
# RSANetWitnessEDR

The RSA NetWitness EDR product is an endpoint threat detection solution that exposes malware and other threats, highlights suspicious activity for investigation, and instantly determines the scope of a compromise to help security teams stop advanced threats faster.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|None|False|IP_OR_HOST|https://<ip>:9443|
|Username|None|False|String||
|Password|None|False|Password|*****|
|Verify SSL|None|False|Boolean|True|


#### Dependencies
| |
|-|
|chardet-5.2.0-py3-none-any.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|idna-3.8-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|
|certifi-2024.8.30-py3-none-any.whl|


## Actions
#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Add IP To Blacklist
Add IP To Blacklist in RSA Netwitness EDR.
Timeout - 600 Seconds



#### Add URL To Blacklist
Add URL To Blacklist in RSA Netwitness EDR.
Timeout - 600 Seconds



#### Enrich Endpoint
Fetch endpoint's system information by its hostname or IP address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|IIOC Score Threshold|Specify IIOC score threshold for the endpoint. If the endpoint exceeds the threshold, the related entity will be marked as suspicious. If nothing is specified, action won’t check the IIOC score.|False|String|50|
|Include IOC Information|If enabled, action will fetch information about the IOCs that are associated with the endpoint|False|Boolean|False|
|Max IOCs To Return|Specify how many IOCs to return. Maximum is 50. This is RSA Netwitness EDR limitation.|False|String|50|



#### Get IOC Details
Enrich Siemplify Entities with information about IOCs from RSA Netwitness EDR.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|IOC Level Threshold|Specify IOC level threshold for the entity. If the entity exceeds the threshold, the related entity will be marked as suspicious.|True|List|Medium|









