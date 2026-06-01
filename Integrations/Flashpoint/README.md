
# Flashpoint

Flashpoint is a global trusted leader in risk intelligence for organizations. From bolstering cyber and physical security, to detecting fraud and insider threats. 
Flashpoint enables users to enrich and enhance their internal data with our targeted data acquired from highly-curated sources.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Key|API Key|True|Password|*****|


#### Dependencies
| |
|-|
|certifi-2025.6.15-py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|idna-3.10-py3-none-any.whl|
|urllib3-2.5.0-py3-none-any.whl|
|charset_normalizer-3.4.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|


## Actions
#### Custom Query
Custom query
See the documentation: "https://docs.fp.tools/"
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Query Content|The content of the query to search.|True|Code|{
  "query": "malcious",
  "limit": "100",
  "start_date": "2020-02-26T14:49:07Z",
  "end_date": "2020-11-26T14:49:07Z",
  "search_tags": "malware",
  "sort_timestamp": "des"
}|
|New Query URL|The new query URL path./all/search|True|String|/all/search|



##### JSON Results
```json
[{"Attribute": [{"category": "string", "comment": "string", "fpid": {}, "href": {}, "timestamp": 0, "type": "string", "uuid": "string", "value": {}}], "RelatedEvent": {}, "Tag": [{"name": "string"}], "attribute_count": 0, "date": "string", "event_creator_email": "string", "href": "string", "uuid": "string"}]
```



#### Indicators Custom Query
Custom query for specific indicators (events and attributes)
See the documentation: "https://docs.fp.tools/#!/indicators/"
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Sort By Time|Presents the data in a descending or ascending order.|False|List|Descending|
|Entity Types|Entity types to retrieve data for (comma separated)For example: url,domain,ip-src.More info : https://www.circl.lu/doc/misp/categories-and-types/|False|String|url,domain,ip-src|
|Limit|The maximum number of result objects to return.|False|String|10|
|Start Date|Retrieves values created after the specified date. For example: 2020-02-26T14:49:07ZFor more info: https://docs.fp.tools/|False|String|2020-02-26T14:49:07Z|
|End Date|Retrieves values created before the specified date. For example: 2020-11-25T14:49:07ZFor more info:https://docs.fp.tools/|False|String|2020-02-25T14:49:07Z|
|Search Tags|Search for a specific keyword (comma separated).For example: malware,ransomware.|False|String|malware,ransomware|
|Query|Custom query to retrieve data for.For example:For more info:|False|String|malicious|
|Indicator Type|Simple-simplified list of indicators of compromiseAttribute- indicators of compromise (IOCs)Event- groupings of different indicators of compromise.|True|List|attribute|



##### JSON Results
```json
[{"Attribute": [{"category": "string", "comment": "string", "fpid": {}, "href": {}, "timestamp": 0, "type": "string", "uuid": "string", "value": {}}], "RelatedEvent": {}, "Tag": [{"name": "string"}], "attribute_count": 0, "date": "string", "event_creator_email": "string", "href": "string", "uuid": "string"}]
```



#### IOC_Enrichment
Enrich indicator attribute Entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Limit|The maximum number of result objects to return.|False|String|100|



##### JSON Results
```json
{}
```



#### Run Query

Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Query|Query content, for example:+{basetypes}:{the basetypes you want to search for}This query search for blog posts that were posted in the past year|True|String|"+basetypes:+indicator"|
|Results count limit|The amount limit of the results.|False|String|100|
|Sort By|Sort by the given fields, for example:"posted_at : desc, title : asc"|False|String|"posted_at:desc,title:as"|
|Tags|A comma separated  list of tags for filtering, for example:tags = +tag_1, +tag_2will return all documents which: have both tag_1 and tag_2 |False|String|+tag_1,+tag2|
|Date Range|The dates range to present the data, for example:+nist.updated_at.date-time:​[now-30d TO now]Note: see date fields table|False|String|[now-1y TO now]|



##### JSON Results
```json
{}
```



#### Ping
Test connectivity with Flashpoint
Timeout - 600 Seconds



##### JSON Results
```json
{}
```









## Connectors
#### Flashpoint - Compromised Credential Connector
Flash Point Connector - Credentials Sighting.
Each time the credentials of an employee in your company are used in the web, alerts will be ingested into Siemplify.


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Key|API Key|True|Password|*****|
|DeviceProductField|The field name used to determine the device product|True|String|case_info.device_product|
|EventClassId|The field name used to determine the event name (sub-type)|False|String|event_name|
|Limit|The limit of the events to retrieve|True|Integer|4|
|Max Days Back|The max days back to retrieve data from|False|Integer|100|
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|PythonProcessTimeout|The timeout limit (in seconds) for the python process running current script|True|String|60|




