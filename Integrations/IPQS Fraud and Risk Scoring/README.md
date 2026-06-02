
# IPQS Fraud and Risk Scoring

IPQS Fraud and Risk Scoring provides enterprise grade fraud prevention, risk analysis, and threat detection. Analyze IP addresses, email addresses, and URLs or domains to identify sophisticated bad actors and high risk behavior.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Key|IPQualityScore API Key|True|Password|*****|


#### Dependencies
| |
|-|
|requests-2.32.4-py3-none-any.whl|
|idna-3.10-py3-none-any.whl|
|certifi-2025.6.15-py3-none-any.whl|
|charset_normalizer-3.4.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl|
|urllib3-2.5.0-py3-none-any.whl|


## Actions
#### Enrich Phone
This action accurately verify phone numbers worldwide and retrieve a combination of carrier and line type details with risk analysis data to assess phone number reputation. IPQS collects phone validation and verification data from a wide variety of carriers and tier 1 telecommunication providers, with support for all regions. Detect inactive and disconnected phone numbers for easy user validation similar to HLR & LRN lookups. Accurately identify virtual and disposable phone numbers along with numbers associated with abusive behavior online.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Strictness|How in depth (strict) do you want this reputation check to be? Stricter checks may provide a higher false-positive rate.|True|List|0|
|Country(For multiple countries, provide comma-separated values)|You can optionally provide us with the default country or countries(comma separated) this phone number is suspected to be associated with.|False|String|None|



#### Enrich Domain
This action Scans links and domains in real-time to detect suspicious URLs using trusted machine learning models. These machine learning models can accurately identify phishing links, malware URLs, viruses, parked domains, and suspicious URLs with real-time risk scores. In addition, the machine learning models can confidently classify poor reputation domains, suspicious links, and phishing URLs with a real-time API integration. Features such as parking domain detection, domain spam scores, reputation checks, and domain age, elevates URL intelligence to a whole new level.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Strictness|How strict should we scan this URL? Stricter checks may provide a higher false-positive rate.|True|List|0|
|Fast|When enabled, the API will provide quicker response times using lighter checks and analysis.|False|Boolean|false|



#### Ping
This action will test the connectivity to the IPQS server.
Timeout - 600 Seconds



#### Enrich URL
This action Scans links and domains in real-time to detect suspicious URLs using trusted machine learning models. These machine learning models can accurately identify phishing links, malware URLs, viruses, parked domains, and suspicious URLs with real-time risk scores. In addition, the machine learning models can confidently classify poor reputation domains, suspicious links, and phishing URLs with a real-time API integration. Features such as parking domain detection, domain spam scores, reputation checks, and domain age, elevates URL intelligence to a whole new level.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Strictness|How strict should we scan this URL? Stricter checks may provide a higher false-positive rate.|True|List|0|
|Fast|When enabled, the API will provide quicker response times using lighter checks and analysis.|False|Boolean|false|



#### Enrich IP
This action performs real-time lookups to instantly determine how risky a user, click, or transaction is based on an IP address and optional device information. In addition to analyzing if the IP address is a proxy or VPN, the API returns over 20 relevant data points such as: Geo location data, ISP, Connection type, Device details, Recent reputation activity, Overall fraud score, Status as a proxy, VPN, or TOR connection, Abuse Velocity, Other similar data points to classify reputation and risk.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|User Language|You can optionally provide us with the users language header. This allows us to evaluate the risk of the user as judged in the "fraud_score".|False|String||
|Fast|When this parameter is enabled our API will not perform certain forensic checks that take longer to process.|False|Boolean|false|
|Mobile|You can optionally specify that this lookup should be treated as a mobile device. |False|Boolean|false|
|Allow Public Access Points|Bypasses certain checks for IP addresses from education and research institutions, schools, and some corporate connections.|False|Boolean|false|
|Lighter Penalties|Skip some denylists which can cause false-positives for sensitive audiences.|False|Boolean|false|
|Strictness|How in depth (strict) do you want this query to be? Higher values take longer to process and may provide a higher false-positive rate.|True|List|0|
|User Agent|You can optionally provide us with the user agent string (browser). This allows to see if the user is a bot or running an invalid browser.|False|String||



#### Enrich Email
This action provides real-time email address reputation scoring and validation with hundreds of syntax & DNS checks. The API can be leveraged to determine if the email address inbox exists with the mail service provider and is able to accept new messages. In addition, users can determine if the email address has a poor reputation or has recently been associated with abuse or threats. Additional risk scoring can detect disposable and temporary mail services as well as emails with a history of fraudulent behavior online.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Abuse Strictness|Set the strictness level for machine learning pattern recognition of abusive email addresses with the "recent_abuse" data point.|True|List|0|
|Fast|When this parameter is enabled our API will not perform an SMTP check with the mail service provider, which greatly increases the API speed.|False|Boolean|false|
|Timeout in seconds|Maximum number of seconds to wait for a reply from a mail service provider. |False|String|7|
|Suggest Domain|Force analyze if the email addresses domain has a typo and should be corrected to a popular mail service.|False|Boolean|false|









