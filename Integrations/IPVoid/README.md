
# IPVoid

IPVoid offers a vast range of IP address tools to discover details about IP addresses.IP blacklist check, whois lookup, dns lookup, ping, and more!

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root|None|True|IP_OR_HOST|https://endpoint.apivoid.com|
|Api Key|None|True|Password|*****|
|Use SSL|None|False|Boolean|False|


#### Dependencies
| |
|-|
|beautifulsoup4-4.12.3-py3-none-any.whl|
|soupsieve-2.5-py3-none-any.whl|


## Actions
#### Get Ip Reputation
Scan an IP address through multiple DNS-based blacklists (DNSBL) and IP reputation services, to facilitate the detection of IP addresses involved in malware incidents and spamming activities
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Threshold|IP risk threshold.|True|String|0|



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### WhoIs
Query the Whois database to find information about a particular domain name or an IP address
Timeout - 600 Seconds









