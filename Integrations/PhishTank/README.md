
# PhishTank

PhishTank is an anti-phishing site. The company offers a community-based phish verification system where users submit suspected phishes and other users "vote" if it is a phish or not. It is a free service that makes your Internet safer, faster, and smarter.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Service Url|Service Url|True|String|https://checkurl.phishtank.com/checkurl/|


#### Dependencies
| |
|-|
|certifi-2025.6.15-py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|xmltodict-0.14.2-py2.py3-none-any.whl|
|idna-3.10-py3-none-any.whl|
|xmljson-0.2.1-py2.py3-none-any.whl|
|urllib3-2.5.0-py3-none-any.whl|
|charset_normalizer-3.4.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|


## Actions
#### Check Url
Check if a specific URL is marked as suspicious by the PhishTank Community. The action will add an insight with the result of the action. 
Timeout - 600 Seconds



##### JSON Results
```json
[{"EntityResult": {"url0": {"url": "https://babules.su/", "in_database": "true", "phish_id": "6605240", "phish_detail_page": "http://www.phishtank.com/phish_detail.php?phish_id=6605240", "verified": "true", "verified_at": "2020-06-01T06:25:58+00:00", "valid": "true"}}, "Entity": "HTTPS://WWW.ONLINESERVICETECH.WEBSITE/LINK/L/P70IPXZLZO2CEED77GJMLWWQXFQCJSVQBYNKZZ346JQYYIKTR6QGAMNQW4L-MXXYSSTIHAEIICD-W1IURFSBN6IUMCO4GWZ_1SBG-62FGIZQK3ZPNIST9WGCBTW-62BXD-FJP7TCWFBSQKVUBEVYLIF_DTC6OYGMQFXDSTFNDB_-CFFKQ4AZNFF13ZWONARJ"}]
```



#### Ping
Test connectivity
Timeout - 600 Seconds



##### JSON Results
```json
{}
```









