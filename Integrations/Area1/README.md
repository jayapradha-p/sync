
# Area1

Area 1 Horizon, a cloud-based service that stops phishing attacks across all traffic vectors—email, web, or network. Protects users against phishing emails using a cloud-based MTA or cloud APIs/connectors. Protects users against web-based phishing campaigns through a globally distributed, recursive DNS service. Shut downs phishing attacks at your network edge.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root|None|True|String|https://api.area1security.com/|
|Username|None|True|String||
|Password|None|True|Password|*****|
|Verify SSL|None|False|Boolean||



## Actions
#### Get Recent Indicators
Get recent malicious indicators from Area1.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Seconds Back|Seconds Back|True|String||



##### JSON Results
```json
[{"threat_categories": [{"classification_disposition": ["Unclassified"]}], "threat_name": "Microsoft Favicon Impersonation", "item_name": "lamcdaniel.com/nc_assets/css/12/", "item_type": "url", "first_seen": 1550127499097, "last_seen": 1550134395800}, {"threat_categories": [{"category": ["Universal"], "threat_type": ["Actor Tool"], "classification_disposition": ["Unclassified"]}], "threat_name": "Area 1 Identified Malicious", "item_name": "e039e82c00e4ae0ddc92908c705350ec", "item_type": "filehash", "first_seen": 1550125103575, "last_seen": 1550125103575}]
```



#### Search Indicator
Search indicator on Area 1 by hash, URL, domain, IP, email.
Timeout - 600 Seconds



##### JSON Results
```json
[{"EntityResult": "85f321d7f27916de21992c5284ff632db3db3481", "Entity": "indicator"}, {"EntityResult": "red", "Entity": "tlp"}, {"EntityResult": 80, "Entity": "overall_confidence"}, {"EntityResult": "85f321d7f27916de21992c5284ff632db3db3481", "Entity": "name"}, {"EntityResult": [{"category": ["Universal"], "threat_type": ["Actor Tool"], "classification_disposition": ["Unclassified"]}], "Entity": "threat_categories"}, {"EntityResult": "drizzle", "Entity": "author"}, {"EntityResult": "85f321d7f27916de21992c5284ff632db3db3481", "Entity": "filehash"}, {"EntityResult": 1550125103522, "Entity": "first_detected"}, {"EntityResult": "85f321d7f27916de21992c5284ff632db3db3481", "Entity": "Hash_SHA1"}, {"EntityResult": "Area 1 Identified Malicious", "Entity": "threat_name"}, {"EntityResult": "85f321d7f27916de21992c5284ff632db3db3481", "Entity": "query_term"}, {"EntityResult": "MAICIOUS", "Entity": "disposition"}, {"EntityResult": "file", "Entity": "family"}, {"EntityResult": [{"category": "Indicator Category", "confidence_rating": 80, "intervals": [{"start": 1550120952000, "end": "current"}], "value": "Universal"}], "Entity": "tag_histories"}, {"EntityResult": 1550125103522, "Entity": "first_seen"}, {"EntityResult": [{"type": "Hash_MD5", "name": "e412341be78003526999f77e8728526e"}, {"type": "Hash_SHA256", "name": "61f006012d2bd7f43bc14ecbeb6a7e690f9d68b4b6b396dab5805be2da75c717"}], "Entity": "aliases"}, {"EntityResult": "Hash_SHA1", "Entity": "type"}, {"EntityResult": 1550120950000, "Entity": "last_seen"}]
```



#### Ping
Test Area1 connectivity.
Timeout - 600 Seconds









