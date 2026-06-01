
# Shodan

Shodan is a search engine that lets the user find specific types of computers (webcams, routers, servers, etc.) connected to the internet using a variety of filters. 

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API key||True|Password|*****|
|Verify SSL||False|Boolean||


#### Dependencies
| |
|-|
|TIPCommon-1.0.11-py2.py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|certifi-2026.4.22-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|idna-3.13-py3-none-any.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|


## Actions
#### DNS Resolve
Look up the IP address for the provided list of hostnames.
Timeout - 600 Seconds



##### JSON Results
```json
{"google.com": "1.1.1.1", "bing.com": "1.1.1.1"}
```



#### Get Api Info
Returns information about the API plan belonging to the given API key.
Timeout - 600 Seconds



##### JSON Results
```json
{"https": false, "unlocked": false, "unlocked_left": 0, "telnet": false, "scan_credits": 0, "plan": "oss", "query_credits": 0}
```



#### Scan A Network
Scan a network using Shodan
Timeout - 600 Seconds



#### DNS Reverse
Look up the hostnames that have been defined for the given list of IP addresses
Timeout - 600 Seconds



##### JSON Results
```json
{"146.125.10.5": null, "8.8.8.8": ["google-public-dns-a.google.com"]}
```



#### Search
Search the SHODAN database.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Search Query|Search query; identical syntax to the website. e.g. find Apache webservers located in Germany(apache country:'DE', city:'Berlin')|True|String||
|Facets|A comma-separated list of properties to get summary information on. Property names can also be in the format of 'property:count'. (i.e. country:100, city:5). More information can be found at https://developer.shodan.io/api |False|String||
|Set Minify|Whether to minify the banner and only return the important data|False|Boolean|false|



##### JSON Results
```json
{"matches": [{"timestamp": "2014-01-15T05: 49: 56.283713", "isp": "Vivacom", "data": "@PJL INFO STATUS CODE=35078 DISPLAY=Power Saver ONLINE=TRUE", "port": 9100, "hostnames": [], "location": {"city": null, "region_code": null, "area_code": null, "longitude": 25, "country_code3": "BGR", "country_name": "Bulgaria", "postal_code": null, "dma_code": null, "country_code": "BG", "latitude": 43}, "ip": 3579573318, "domains": [], "org": "Vivacom", "os": null, "asn": "AS8866", "ip_str": "1.1.1.1"}], "facets": {"org": [{"count": 107, "value": "UniversityofMinnesota"}]}, "total": 12039}
```



#### Get Ip Info
Get all available information on an IP
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Return Historical Banners|True if all historical banners should be returned|False|Boolean|false|
|Set Minify|True to only return the list of ports and the general host information, no banners.|False|Boolean|false|



##### JSON Results
```json
[{"EntityResult": {"data": [{"_shodan": {"id": "d670bfbb-4821-4320-969d-0590789ab502", "crawler": "545144fc95e7a7ef13ece5dbceb98ee386b37950", "options": {}, "module": "dns-udp", "ptr": true}, "hash": -553166942, "opts": {"raw": "34ef818200010000000000000756455253494f4e0442494e440000100003"}, "ip": 134744072, "isp": "Google", "data": "\nRecursion: enabled", "port": 53, "hostnames": ["google-public-dns-a.google.com"], "location": {"city": null, "region_code": null, "area_code": null, "dma_code": null, "country_code3": "USA", "country_name": "United States", "postal_code": null, "longitude": -97.822, "country_code": "US", "latitude": 37.751000000000005}, "dns": {"resolver_hostname": null, "recursive": true, "resolver_id": null, "software": null}, "timestamp": "2019-01-29T12:36:09.300695", "domains": ["google.com"], "org": "Google", "os": null, "asn": "AS15169", "transport": "udp", "ip_str": "1.1.1.1"}], "city": null, "region_code": null, "tags": [], "ip": 134744072, "isp": "Google", "area_code": null, "dma_code": null, "last_update": "2019-01-29T12:36:09.300695", "country_code3": "USA", "country_name": "United States", "hostnames": ["google-public-dns-a.google.com"], "postal_code": null, "longitude": -97.822, "country_code": "US", "ip_str": "1.1.1.1", "latitude": 37.751000000000005, "org": "Google", "os": null, "asn": "AS15169", "ports": [53]}, "Entity": "1.1.1.1"}]
```



#### Ping
Test connectivity
Timeout - 600 Seconds



#### SearchForExploits
Search across a variety of data sources for exploits and use facets to get summary information.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Search Query|Search query used to search the database of known exploits.|True|String||
|Facets|A comma-separated list of properties to get summary information on. (i.e. port, source, author). More information can be found at https://developer.shodan.io/api|False|String||
|Page|The page number to page through results 100 at a time.|False|String||



##### JSON Results
```json
{"matches": [{"cve": "CVE-2011-2064", "description": "Cisco IOS 12.4MDA before 12.4(24)MDA5 on the Cisco Content Services Gateway - Second Generation (CSG2) allows remote attackers to cause a denial of service (device reload) via crafted ICMP packets, aka Bug ID CSCtl79577.", "osvdb": [73657], "bid": [48581], "source": "CVE", "_id": "2011-2064", "msb": []}], "facets": {"type": [{"count": 1, "value": "remote"}]}, "total": 4}
```









