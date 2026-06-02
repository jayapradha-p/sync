
# Cloudflare

Cloudflare is a global cloud services provider that delivers a broad range of services to businesses of all sizes and in all geographies—making them more secure, enhancing the performance of their business-critical applications, and eliminating the cost and complexity of managing individual network hardware.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|API root of the Cloudflare instance.|True|String|https://api.cloudflare.com|
|API Token|API Token of the Cloudflare instance.|True|Password|*****|
|Account Name|Name of the account that needs to be used in the integration.|True|String||
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Cloudflare server is valid.|False|Boolean|true|


#### Dependencies
| |
|-|
|requests-2.32.4-py3-none-any.whl|
|idna-3.13-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|certifi-2026.4.22-py3-none-any.whl|
|TIPCommon-1.0.12-py2.py3-none-any.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|


## Actions
#### Add IP To Rule List
Add IP addresses to the rule list in Cloudflare. Supported Entities: IP Address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Rule Name|Specify the name of the rule list to which you want to add rule list items.|True|String||
|Description|Specify a description for the newly added rule list items.|False|String||



#### List Firewall Rules
List available firewall rules in Cloudflare.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Zone Name|Specify the name of the zone, which will contain the firewall rule.|True|String||
|Filter Key|Specify the key that needs to be used to filter results.|False|List|Select One|
|Filter Logic|Specify what filter logic should be applied. Filtering logic is working based on the value  provided in the "Filter Key" parameter.|False|List|Select One|
|Filter Value|Specify what value should be used in the filter. If "Equal" is selected, action will try to find the exact match among results and if "Contains" is selected, action will try to find results that contain that substring. If nothing is provided in this parameter, the filter will not be applied. Filtering logic is working based on the value provided in the "Filter Key" parameter.|False|String||
|Max Records To Return|Specify how many records to return. If nothing is provided, action will return 50 records.|False|String|50|



#### Add URL To Rule List
Add URLs to the rule list in Cloudflare. Supported Entities: URL. Note: URL entities are treated as "Source URLs".
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Rule Name|Specify the name of the rule list to which you want to add rule list items.|True|String||
|Target URL|Specify the target URL for the rule list item.|True|String||
|Description|Specify a description for the newly added rule list item.|False|String||
|Status Code|Specify the status for the rule list item.|False|List|301|
|Preserve Query String|If enabled, the rule list item will preserve the query string.|False|Boolean|false|
|Include Subdomains|If enabled, the rule list item will include subdomains.|False|Boolean|false|
|Subpath Matching|If enabled, the rule list item will match the subpath.|False|Boolean|false|
|Preserve Path Suffix|If enabled, the rule list item will preserve the path suffix.|False|Boolean|false|



#### Ping
Test connectivity to the Cloudflare with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Update Firewall Rule
Update a firewall rule in Cloudflare.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Rule Name|Specify the name of the rule that needs to be updated.|True|String||
|Zone Name|Specify the name of the zone, which will contain the firewall rule.|True|String||
|Action|Specify the action for the firewall rule. If "Bypass" is selected, you need to provide values in the "Products" parameter.|False|List|Block|
|Expression|Specify the expression for the firewall rule.|False|String||
|Products|Specify a comma-separated list of products for the firewall rule. Note: this parameter is only mandatory, if "Bypass" is selected for "Action" parameter. Possible values: zoneLockdown, uaBlock, bic, hot, securityLevel, rateLimit, waf.|False|String||
|Priority|Specify the priority for the firewall rule.|False|String||
|Reference Tag|Specify a reference tag for the firewall rule. Note: it can only be up to 50 characters long.|False|String||



#### Create Firewall Rule
Create a firewall rule in Cloudflare.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Zone Name|Specify the name of the zone, which will contain the firewall rule.|True|String||
|Name|Specify the name for the firewall rule.|False|String||
|Action|Specify the action for the firewall rule. If "Bypass" is selected, you need to provide values in the "Products" parameter.|False|List|Block|
|Expression|Specify the expression for the firewall rule.|True|String||
|Products|Specify a comma-separated list of products for the firewall rule. Note: this parameter is only mandatory, if "Bypass" is selected for "Action" parameter. Possible values: zoneLockdown, uaBlock, bic, hot, securityLevel, rateLimit, waf.|False|String||
|Priority|Specify the priority for the firewall rule.|False|String||
|Reference Tag|Specify a reference tag for the firewall rule. Note: it can only be up to 50 characters long.|False|String||



#### Create Rule List
Create a rule list in Cloudflare.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Name|Specify the name for the rule list.|True|String||
|Type|Specify the type for the rule list.|False|List|IP Address|
|Description|Specify the description for the rule list.|False|String||









