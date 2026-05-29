
# MandiantASM

Mandiant Advantage Attack Surface Management automates external asset discovery and analysis to uncover vulnerabilities, misconfigurations and exposures.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|API root of the Mandiant ASM instance. Note: if you want to authenticate with GTI credentials provide "https://www.virustotal.com" as API Root.|True|String|https://asm-api.advantage.mandiant.com|
|Access Key|API Access Key of the Mandiant ASM account|False|String||
|Secret Key|API Secret Key of the Mandiant ASM account.|False|Password|*****|
|GTI API Key|Google Threat Intelligence API Key. Note: API Root should be "https://www.virustotal.com" to use this authentication. GTI API Key authentication has priority over other authentication.|False|Password|*****|
|Project Name|Project name that should be used in Mandiant ASM. If Access Key & Secret Key is used for authentication, this parameter is mandatory.|False|String||
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Mandiant ASM server is valid.|False|Boolean|true|


#### Dependencies
| |
|-|
|TIPCommon-1.0.16-py2.py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|EnvironmentCommon-1.0.2-py2.py3-none-any.whl|
|idna-3.8-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|
|certifi-2024.8.30-py3-none-any.whl|


## Actions
#### Update Issue
Update an issue in Mandiant ASM.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Issue ID|Specify the ID of the issue that needs to be updated.|True|String|None|
|Status|Specify what status to set for the issues.|True|List|Select One|



##### JSON Results
```json
{"uuid": "9f715a20-5b9b-4c7c-a5c8-2c210402d80d", "dynamic_id": 31723111, "entity_uid": "70fca9e430435258e59d4ecbf057b76181debfedf8544b95fd6c5eb740faf044", "alias_group": "975418", "category": "misconfiguration", "confidence": "confirmed", "description": "This certificate will expire in 30 days or less.", "details": {"name": "invalid_certificate_almost_expired", "added": "2020-08-20", "proof": "Not Valid after 2023-03-06 20:32:44 UTC which is less than the warning window of: 5 days", "status": "confirmed", "category": "misconfiguration", "severity": 3, "references": [], "description": "This certificate will expire in 30 days or less.", "pretty_name": "(Almost) Expired Certificate", "remediation": "Replace the certificate and/or de-provision the service"}, "first_seen": "2023-03-06T21:05:17.000Z", "identifiers": null, "last_seen": "2023-03-06T21:05:17.000Z", "name": "invalid_certificate_almost_expired", "pretty_name": "(Almost) Expired Certificate", "scoped": true, "severity": 3, "source": "intrigue", "status": "open_in_progress", "ticket_list": [], "type": "standard", "uid": "65af0677bd415c484a1d7761881c580c054e6eed7f2c76eb2d46be8b0295c5d2", "upstream": "intrigue", "created_at": "2023-03-06T21:08:07.550Z", "updated_at": "2023-04-06T14:41:44.739Z", "entity_id": 335047476, "collection_id": 32538, "elasticsearch_mappings_hash": "dde64e2cef94909a0498d10293808b84", "collection": "mandiant", "collection_type": "pre_collection", "collection_uuid": "a8de4539-f269-447b-81fb-0ee1770e982f", "organization_uuid": null, "entity_name": "asm-vulndb.core-stage.asm.mandiant.com (270360015250059971284494692029118798042890)", "entity_type": "Intrigue::Entity::SslCertificate", "summary": {"pretty_name": "(Almost) Expired Certificate", "severity": 3, "scoped": true, "confidence": "confirmed", "status": "open_in_progress", "category": "misconfiguration", "identifiers": null, "status_new": "open", "status_new_detailed": "in_progress", "ticket_list": []}, "tags": []}
```



#### Ping
Test connectivity to the MandiantASM with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Get ASM Entity Details
Return information about a Mandiant ASM entity.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Entity IDs|Specify a comma-separated list of entity IDs for which you want to fetch details.|True|String|None|



##### JSON Results
```json
[{"uuid":"6464030e-xxxxxxxxxxxxxxxx","dynamic_id":"Intrigue::Entity::Uri#http://3.0.xxx.xxx","collection_name":"awsdemorange_xxxxxxxx","alias_group":"4d289xxxxxxxxxxxxxxxxxxxxxxxxx","aliases":null,"allow_list":false,"ancestors":[{"name":"3.0.xxx.xxx","type":"Intrigue::Entity::NetBlock"}],"category":null,"collection_naics":null,"confidence":null,"deleted":false,"deny_list":false,"details":{"asn":null,"ssl":false,"uri":"http://3.0.xxx.xxx","code":"404","port":80,"forms":false,"title":"404 Not Found","verbs":null,"cookies":null,"headers":["Date: Fri, 30 Sep 2022 06:51:11 GMT","Content-Type: text/html","Content-Length: 548","Connection: keep-alive"],"host_id":1111111,"net_geo":"US","scripts":[],"service":"http","auth.2fa":false,"auth.any":false,"dom_sha1":"540707xxxxxxxxxxxxxxxxxxxxxxxx","net_name":"","protocol":"tcp","alt_names":null,"auth.ntlm":false,"generator":null,"auth.basic":false,"auth.forms":false,"ip_address":"3.0.xxx.xxx","favicon_md5":null,"fingerprint":[{"cpe":"cpe:2.3:a:nginx:nginx::","hide":false,"tags":["Web Server"],"type":"fingerprint","tasks":null,"issues":null,"method":"ident","update":null,"vendor":"Nginx","product":"Nginx","version":null,"inference":false,"description":"nginx (default page)","match_logic":"all","positive_matches":[{"match_type":"content_body","match_content":"(?i-mx:<hr><center>nginx/?([\\d.]*)</center>)"}]},{"cpe":"cpe:2.3:a:nginx:nginx::","hide":false,"tags":["Web Server"],"type":"fingerprint","tasks":null,"issues":null,"method":"ident","update":null,"vendor":"Nginx","product":"Nginx","version":null,"inference":false,"description":"nginx (default page - could be redirect)","match_logic":"all","positive_matches":[{"match_type":"content_body","match_content":"(?i-mx:<hr><center>nginx/?[\\d.]*</center>)"}]}],"geolocation":{"asn":{"asn":16509,"isp":"Amazon Technologies Inc.","name":"Amazon.com, Inc.","organization":"Amazon Data Services Singapore","connection_type":"Corporate"},"city":"Singapore","postal":"049481","country":"Singapore","latitude":1.35208,"continent":"Asia","longitude":103.82,"time_zone":"Asia/Singapore","country_code":"SG","continent_code":"AS"},"vuln_checks":["log4shell_cve_2021_44228"],"api_endpoint":false,"cloud_hosted":true,"favicon_sha1":null,"domain_cookies":null,"log4shell_uuid":"55be32xxxxxxxxxxxxxxxxxxxxx","redirect_chain":[],"redirect_count":0,"cloud_providers":["Amazon Web Services"],"net_country_code":null,"screenshot_exists":true,"cloud_fingerprints":[],"response_data_hash":"1GUXIXXxxxxxxxxxxxxxxxxxxxxxxxx","exfil_lookup_identifier":"55be32xxxxxxxxxxxxxxxxxxxxxxxxxx"},"details_file":"xxxxxxxxxxxxxxxxxxxxxx.json","description":null,"first_seen":"2022-09-30T21:20:19.000Z","hidden":false,"last_seen":"2022-09-30T21:20:19.000Z","name":"http://3.0.216.73:80","scoped":true,"scoped_reason":"entity_scoping_rules: fallback value","seed":null,"source":null,"status":null,"task_results":[{"name":"search_shodan_on_3.0.xx.xxx","task":"search_shodan","depth":4,"entity_name":"3.0.xx.xxx","entity_type":"Intrigue::Entity::NetBlock"},{"name":"port_scan_on_3.0.xxx.xxx","task":"port_scan","depth":3,"entity_name":"3.0.xxx.xxx","entity_type":"Intrigue::Entity::IpAddress"}],"type":"Intrigue::Entity::Uri","uid":"9bae9d6xxxxxxxxxxxxxxxxxxxxxx","created_at":"2022-09-30T21:25:05.232Z","updated_at":"2022-09-30T21:25:05.239Z","collection_id":117139,"elasticsearch_mappings_hash":null,"collection":"awsdemorange_oum28bu","collection_uuid":"51131xxxxxxxxxxxxxxxxxxxxxxxx","organization_uuid":"21d2xxxxxxxxxxxxxxxxxxxxxxx","collection_type":"user_collection","fingerprint":[{"cpe":"cpe:2.3:a:nginx:nginx::","hide":false,"tags":["Web Server"],"type":"fingerprint","tasks":null,"issues":null,"method":"ident","update":null,"vendor":"Nginx","product":"Nginx","version":null,"inference":false,"description":"nginx (default page)","match_logic":"all","positive_matches":[{"match_type":"content_body","match_content":"(?i-mx:<hr><center>nginx/?([\\d.]*)</center>)"}],"local_icon_path":"/assets/fingerprints/nginx.png"},{"cpe":"cpe:2.3:a:nginx:nginx::","hide":false,"tags":["Web Server"],"type":"fingerprint","tasks":null,"issues":null,"method":"ident","update":null,"vendor":"Nginx","product":"Nginx","version":null,"inference":false,"description":"nginx (default page - could be redirect)","match_logic":"all","positive_matches":[{"match_type":"content_body","match_content":"(?i-mx:<hr><center>nginx/?[\\d.]*</center>)"}],"local_icon_path":"/assets/fingerprints/nginx.png"}],"summary":{"scoped":true,"issues":{"current_with_cve":0,"current_by_severity":{"1":1},"all_time_by_severity":{"1":1},"current_count":1,"all_time_count":1,"critical_or_high":true},"task_results":["search_shodan","port_scan","port_scan_lambda","search_shodan"],"screenshot_exists":true,"geolocation":{"city":"Singapore","country_code":"SG","country_name":null,"latitude":1.35208,"longitude":103.82,"asn":null},"http":{"code":404,"title":"404 Not Found","content":{"favicon_hash":null,"hash":null,"forms":false},"auth":{"any":false,"basic":false,"ntlm":false,"forms":false,"2fa":false}},"ports":{"tcp":[80],"udp":[],"count":1},"network":{"name":"Amazon.com, Inc.","asn":16509,"route":null,"type":null},"technology":{"cloud":true,"cloud_providers":["Amazon Web Services"],"cpes":[],"technologies":[],"technology_labels":[]},"vulns":{"current_count":0,"vulns":[]}},"tags":[]}]
```



#### Search Issues
Search Issues that match the specified criteria in the action Parameters.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Issue IDs|Specify a comma-separated list of issue ids, for which you want to return details.|False|String|None|
|Entity IDs|Specify a comma-separated list of entity ids for which you want to find related issues.|False|String|None|
|Entity Name|Specify a comma-separated list of entity names for which you want to find related issues.|False|String|None|
|Time Parameter|Specify what parameter should be used for filtering time.|False|List|First Seen|
|Time Frame|Specify a time frame for the issues. If “Custom” is selected, you also need to provide “Start Time”.|False|List|Last Hour|
|Start Time|Specify the start time for the results. This parameter is mandatory, if “Custom” is selected for the “Time Frame” parameter. Format: ISO 8601|False|String|None|
|End Time|Specify the end time for the results. Format: ISO 8601. If nothing is provided and “Custom” is selected for the “Time Frame” parameter then this parameter will use current time.|False|String|None|
|Lowest Severity To Return|Specify the lowest severity that should be used to return the issues. If “Select One” is selected, this filter is not applied during the search.|False|List|Select One|
|Status|Specify the status filter for the search. If “Select One” is selected, this filter is not applied during the search.|False|List|Select One|
|Tags|Specify a comma-separated list of tag names, which should be used, when searching for the issues.|False|String|None|
|Max Issues To Return|Specify how many issues to return. Default: 50. Maximum is 200.|False|String|50|



##### JSON Results
```json
[{"id": "xxxxxxxx", "uuid": "89d68a35-ba7b-47b7-825c-e7febe611f4b", "dynamic_id": 2867262, "name": "self_signed_certificate", "upstream": "intrigue", "last_seen": "2022-03-03T21:00:04.000Z", "first_seen": "2022-03-03T21:00:04.000Z", "entity_uid": "e1f175c3c7568570caa0c7855801c08bb30cdb0de7756746905617893f086559", "entity_type": "Intrigue::Entity::Uri", "entity_name": "https://3.214.213.33:443", "alias_group": "13372361", "collection": "mandiant", "collection_uuid": "a8de4539-f269-447b-81fb-0ee1770e982f", "collection_type": "pre_collection", "organization_uuid": null, "summary": {"pretty_name": "Self Signed Certificate Detected", "severity": 5, "scoped": true, "confidence": "confirmed", "status": null, "category": "misconfiguration", "identifiers": null, "status_new": "closed", "status_new_detailed": null, "ticket_list": null}, "tags": []}]
```



#### Search ASM Entities
Search entities in Mandiant ASM.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Entity Name|Specify a comma-separated list of entity names for which you want to find entities.|False|String|None|
|Critical or High Issue|Specify whether to include only entities with High or Critical Issues.|False|Boolean|false|
|Minimum Vulnerabilities Count|Specify how many vulnerabilities should be related to the entity for it to be returned.|False|String||
|Minimum Issues Count|Specify how many issues should be related to the entity for it to be returned.|False|String||
|Tags|Specify a comma-separated list of tag names, which should be used, when searching for the entities.|False|String|None|
|Max Entities To Return|Specify how many entities to return. Default: 50. Maximum is 200.|False|String|50|



##### JSON Results
```json
  [{  
    "Entity": "entity_name",  
    "EntityResult": {  
      "id": "e947ffd19081586e8e2aafef0db2fdafd7b4d764ff5203cedb8ac2bae8c9b14f",  
      "dynamic_id": "Intrigue::Entity::ApiEndpoint#entity_name",  
      "alias_group": "207281",  
      "name": "entity_name",  
      "type": "Intrigue::Entity::ApiEndpoint",  
      "first_seen": "2021-09-03T17:03:38Z",  
      "last_seen": "2021-09-03T17:03:38Z",  
      "collection": "mandiant",  
      "collection_type": "Intrigue::Collections::PreCollection",  
      "collection_naics": ["541512", "561685"],  
      "collection_uuid": "a8de4539-f269-447b-81fb-0ee1770e871f",  
      "organization_uuid": null,  
      "tags": [],  
      "issues": [],  
      "exfil_lookup_identifier": null,  
      "summary": {  
        "scoped": true,  
        "issues": {  
          "current_by_severity": {},  
          "current_with_cve": 0,  
          "all_time_by_severity": {},  
          "current_count": 0,  
          "all_time_count": 0,  
          "critical_or_high": false  
        },  
        "task_results": ["uri_check_api_endpoint"],  
        "screenshot_exists": false,  
        "http": {  
          "code": 403,  
          "title": null,  
          "content": { "favicon_hash": null, "hash": null, "forms": null },  
          "auth": {  
            "any": null,  
            "basic": null,  
            "ntlm": null,  
            "forms": null,  
            "2fa": null  
          }  
        },  
        "ports": { "count": 0, "tcp": null, "udp": null },  
        "technology": { "cloud": false, "cloud_providers": [] },  
        "network": { "name": null, "asn": null, "route": null, "type": null }  
      }  
    }  
  },  
  {  
    "Entity": "entity_name2",  
    "EntityResult": {  
      "id": "20f65f6175a73d9aee82b4dbcbcd245c94ac5b9e1aae25c2ad3c322284c9a8b8",  
      "dynamic_id": "Intrigue::Entity::Uri#entity_name2",  
      "alias_group": "cbeb42a84fb7c6e48e88",  
      "name": "entity_name2",  
      "type": "Intrigue::Entity::Uri",  
      "first_seen": "2021-09-03T17:03:38Z",  
      "last_seen": "2021-09-03T17:03:38Z",  
      "collection": "mandiant",  
      "collection_type": "Intrigue::Collections::PreCollection",  
      "collection_naics": ["541511", "561621"],  
      "collection_uuid": "a8de3539-f269-447b-81fb-0ee1770e982f",  
      "organization_uuid": null,  
      "tags": [],  
      "issues": [],  
      "exfil_lookup_identifier": null,  
      "summary": {  
        "scoped": true,  
        "issues": {  
          "current_by_severity": {},  
          "current_with_cve": 0,  
          "all_time_by_severity": {},  
          "current_count": 0,  
          "all_time_count": 0,  
          "critical_or_high": false  
        },  
        "task_results": ["search_shodan"],  
        "screenshot_exists": false,  
        "geolocation": {  
          "city": null,  
          "country_code": "US",  
          "country_name": null,  
          "latitude": null,  
          "asn": null  
        },  
        "http": {  
          "code": 200,  
          "title": "FireEye Threat Intelligence",  
          "content": { "favicon_hash": null, "hash": null, "forms": false },  
          "auth": {  
            "any": false,  
            "basic": false,  
            "ntlm": false,  
            "forms": true,  
            "2fa": false  
          }  
        },  
        "ports": { "count": 1, "tcp": ["80"], "udp": null },  
        "network": { "name": "DATE", "asn": null, "route": null, "type": null },  
        "technology": {  
          "cloud": true,  
          "cloud_providers": ["threat intelligence"]  
        },  
        "vulns": { "current_count": 0, "vulns": [] }  
      }  
    }  
  }  
]  

```









## Connectors
#### Mandiant ASM - Issues Connector
Pull information about issues from Mandiant ASM. Note: The Dynamic List filter works with the "category" parameter.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|DeviceProductField|Enter the source field name in order to retrieve the Product Field name.|True|String|Product Name|
|EventClassId|Enter the source field name in order to retrieve the Event Field name.|True|String|entity_type|
|PythonProcessTimeout|Timeout limit for the python process running the current script.|True|Integer|180|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|API Root|API root of the Mandiant ASM instance. Note: if you want to authenticate with GTI credentials provide “https://www.virustotal.com” as API Root.|True|String|https://asm-api.advantage.mandiant.com|
|Access Key|API Access Key of the Mandiant ASM account.|False|Password|*****|
|Secret Key|API Secret Key of the Mandiant ASM account.|False|Password|*****|
|GTI API Key|Google Threat Intelligence API Key. Note: API Root should be “https://www.virustotal.com” to use this authentication. GTI API Key authentication has priority over other authentication.|False|Password|*****|
|Project Name|Project name that should be used in Mandiant ASM.  If Access Key & Secret Key is used for authentication, this parameter is mandatory.|False|String||
|Lowest Severity To Fetch|Lowest severity that needs to be used to fetch issues. Possible values: Informational, Low, Medium, High, Critical. If nothing is specified, the connector will ingest issues with all severities.|False|String||
|Max Hours Backwards|Number of hours before the first connector iteration to fetch issues from. This parameter applies to the initial connector iteration after you enable the connector for the first time, or used as a fallback value in cases where connector's last run timestamp expires.|False|Integer|1|
|Max Issues To Fetch|Specify the number of issues to process per one connector iteration. Default: 10.|False|Integer|10|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Mandiant ASM server is valid.|False|Boolean|true|
|Use dynamic list as a blocklist|If enabled, dynamic lists will be used as a blocklist.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




