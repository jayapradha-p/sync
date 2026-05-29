
# ThreatQ

A threat intelligence platform designed to accelerate security operations.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|ServerAddress|None|True|IP|xx.xx.xx.xx|
|ClientId|None|True|String||
|Username|None|True|String||
|Password|None|True|Password|*****|


#### Dependencies
| |
|-|
|chardet-5.2.0-py3-none-any.whl|
|requests-2.31.0-py3-none-any.whl|
|certifi-2024.2.2-py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|idna-3.7-py3-none-any.whl|
|urllib3-2.2.1-py3-none-any.whl|
|TIPCommon-1.0.11-py2.py3-none-any.whl|


## Actions
#### Create Object
Create an object in ThreatQ.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Object Type|Specify to which object type attribute should be added.|True|List|Attack Pattern|
|Value|Specify the value of the new object.|True|String||
|Description|Specify description of the new object.|False|String||



#### Enrich Hash
Enrich a Hash using ThreatQ information.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Score Threshold|Set the acceptable score threshold for the entity. If the score exceeds the specified threshold, entity will be marked as suspicious.|False|String|5|
|Show Sources|If enabled, action will return an additional table with related sources.|False|Boolean|true|
|Show Comments|If enabled, action will return an additional table with related comments.|False|Boolean|true|
|Show Attributes|If enabled, action will return an additional table with related attributes.|False|Boolean|true|
|Mark Whitelisted Entities As Suspicious|If enabled, action will mark entities as suspicious if they passed the allowed threshold, even if the entity is whitelisted in ThreatQ.|False|Boolean|true|



#### Enrich URL
Enrich an URL using ThreatQ information.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Score Threshold|Set the acceptable score threshold for the entity. If the score exceeds the specified threshold, entity will be marked as suspicious.|False|String|5|
|Show Sources|If enabled, action will return an additional table with related sources.|False|Boolean|true|
|Show Comments|If enabled, action will return an additional table with related comments.|False|Boolean|true|
|Show Attributes|If enabled, action will return an additional table with related attributes.|False|Boolean|true|
|Mark Whitelisted Entities As Suspicious|If enabled, action will mark entities as suspicious if they passed the allowed threshold, even if the entity is whitelisted in ThreatQ.|False|Boolean|true|



#### Link Objects
Action links two objects in ThreatQ.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Source Object Type|Specify the type of the source object.|True|List|Adversary|
|Source Object Identifier|Specify identifier of the source object. For example, it can be an MD5 hash, title of the event, name of the adversary etc.|True|String||
|Source Indicator Type|Specify the type of the source indicator. This parameter is only used, if Source Object Type is Indicator.|False|List||
|Destination Object Type|Specify the type of the destination object.|True|List|Adversary|
|Destination Object Identifier|Specify identifier of the destination object. For example, it can be an MD5 hash, title of the event, name of the adversary etc.|True|String||
|Destination Indicator Type|Specify the type of the destination indicator. This parameter is only used, if Destination Object Type is Indicator.|False|List||



#### List Entity Related Objects
Action lists related objects for entities in ThreatQ.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Related Object Type|Specify the type of the related object that needs to be returned.|True|List|Adversary|
|Max Related Objects To Return|Specify how many related objects to return. Maximum is 1000. This is a ThreatQ limitation.|False|String|50|



#### Create Adversary
Create an adversary in ThreatQ.
Timeout - 600 Seconds



#### Update Indicator Score
Action updates indicator score in ThreatQ
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Score|Specify the new score of the indicator.|True|List|7 - Medium|
|Score Validation|Specify what kind of score validation should be used. If “ Highest Score” is specified, action will compare current values and update the indicator’s score only, if the specified score is higher than current generated and manual score. If “Force Update” is specified, action will update the indicator's score without comparing current values.|True|List|Highest Score|



#### Add Attribute
Action adds an attribute to the object.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Object Type|Specify to which object type attribute should be added.|True|List|Adversary|
|Object Identifier|Specify identifier of the object. For example, it can be an MD5 hash, title of the event, name of the adversary etc.|True|String||
|Indicator Type|Specify the type of the indicator. This parameter is only used, if Source Object Type is Indicator.|False|List|ASN|
|Attribute Name|Specify the name of the attribute.|True|String||
|Attribute Value|Specify the value of the attribute.|True|String||
|Attribute Source|Specify the source of the attribute.|False|String||



#### Enrich CVE
Enrich a CVE using ThreatQ information.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Score Threshold|Set the acceptable score threshold for the entity. If the score exceeds the specified threshold, entity will be marked as suspicious.|False|String|5|
|Show Sources|If enabled, action will return an additional table with related sources.|False|Boolean|true|
|Show Comments|If enabled, action will return an additional table with related comments.|False|Boolean|true|
|Show Attributes|If enabled, action will return an additional table with related attributes.|False|Boolean|true|
|Mark Whitelisted Entities As Suspicious|If enabled, action will mark entities as suspicious if they passed the allowed threshold, even if the entity is whitelisted in ThreatQ.|False|Boolean|true|



#### Create Event
Create an event in ThreatQ.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Event Type|Specify the type of the event.|True|List|Spearphish|
|Title|Specify the title of the event.|True|String||
|Happened At|Specify when the event happened. If nothing is entered in this field, action will use current time. Format: YYYY-MM-DD hh:mm:ss|False|String||



#### Enrich Email
Enrich an email address using ThreatQ information.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Score Threshold|Set the acceptable score threshold for the entity. If the score exceeds the specified threshold, entity will be marked as suspicious.|False|String|5|
|Show Sources|If enabled, action will return an additional table with related sources.|False|Boolean|true|
|Show Comments|If enabled, action will return an additional table with related comments.|False|Boolean|true|
|Show Attributes|If enabled, action will return an additional table with related attributes.|False|Boolean|true|
|Mark Whitelisted Entities As Suspicious|If enabled, action will mark entities as suspicious if they passed the allowed threshold, even if the entity is whitelisted in ThreatQ.|False|Boolean|true|



#### Get Indicator Details
Search for entities in ThreatQ and get detailed information.
Timeout - 600 Seconds



#### Link Entities
Action links all of the entities in ThreatQ.
Timeout - 600 Seconds



#### List Events
List events from ThreatQ.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Additional Fields|Specify what additional fields should be included in the response. Possible values: adversaries, attachments, attributes, comments, events, indicators, signatures, sources, spearphish, tags, type, watchlist.|False|String|adversaries, attachments, attributes, comments, events, indicators, signatures, sources, spearphish, tags, type, watchlist|
|Sort Field|Specify what field should be used for sorting events.|False|List|ID|
|Sort Direction|Specify the sorting direction.|False|List|Ascending|
|Max Events To Return|Specify how many events to return.|False|String|50|



#### Update Indicator Status
Action updates indicator status in ThreatQ.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Status|Specify the new status of the indicator.|True|List|Active|



#### Get Malware Details
Action returns information about malware based on entities from ThreatQ.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Additional Information|Specify what additional fields should be included in the response. Possible values: adversaries, attackPattern, campaign, courseOfAction, attachments, attributes, comments, events, indicators, signatures, sources, status, tags, type, watchlist, exploitTarget, identity, incident, intrusionSet, malware, report, tool, ttp, vulnerability, tasks|False|String|adversaries,attackPattern,campaign,courseOfAction,attachments,attributes,comments,events,indicators,signatures,sources,status,tags,type,watchlist,exploitTarget,identity,incident,intrusionSet,malware,report,tool,ttp,vulnerability,tasks|



#### Link Entities To Object
Action links all of the entities in ThreatQ.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Object Type|Specify the type of the object to which you want to link entities.|True|List|Adversary|
|Object Identifier|Specify identifier of the object to which you want to link entities. For example, it can be an MD5 hash, title of the event, name of the adversary etc.|True|String||
|Indicator Type|Specify the type of the  indicator to which you want to link entities. This parameter is only used, if Source Object Type is “Indicator”.|False|List|ASN|



#### Create Indicator
Create an indicator in ThreatQ.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Indicator Type|Specify the type of the new indicator.|True|List|ASN|
|Status|Specify the status of the new indicator.|True|List|Active|
|Description|Specify description of the new indicator.|False|String||



#### List Related Objects
Action lists related objects in ThreatQ.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Source Object Type|Specify the type of the source object.|True|List|Adversary|
|Source Object Identifier|Specify identifier of the source object. For example, it can be an MD5 hash, title of the event, name of the adversary etc.|True|String||
|Source Indicator Type|Specify the type of the source indicator. This parameter is only used, if Source Object Type is Indicator.|False|List||
|Related Object Type|Specify the type of the related object that needs to be returned.|True|List|Adversary|
|Max Related Objects To Return|Specify how many related objects to return.|False|String|50|



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Add Source
Action adds a source to the object.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Object Type|Specify to which object type source should be added.|True|List|Adversary|
|Object Identifier|Specify identifier of the object. For example, it can be an MD5 hash, title of the event, name of the adversary etc.|True|String||
|Indicator Type|Specify the type of the indicator. This parameter is only used, if Source Object Type is Indicator.|False|List|ASN|
|Source Name|Specify the name of the source.|True|String||



#### Enrich IP
Enrich an IP using ThreatQ information.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Score Threshold|Set the acceptable score threshold for the entity. If the score exceeds the specified threshold, entity will be marked as suspicious.|False|String|5|
|Show Sources|If enabled, action will return an additional table with related sources.|False|Boolean|true|
|Show Comments|If enabled, action will return an additional table with related comments.|False|Boolean|true|
|Show Attributes|If enabled, action will return an additional table with related attributes.|False|Boolean|true|
|Mark Whitelisted Entities As Suspicious|If enabled, action will mark entities as suspicious if they passed the allowed threshold, even if the entity is whitelisted in ThreatQ.|False|Boolean|true|









