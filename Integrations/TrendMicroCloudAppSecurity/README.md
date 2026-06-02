
# TrendMicroCloudAppSecurity

Trend Micro Cloud App Security enables you to embrace the efficiency of cloud services while maintaining security. It protects incoming and internal Office 365 email from advanced malware and other threats, and enforces compliance on other cloud file-sharing services, including Box, Dropbox, Google Drive, SharePoint® Online, and OneDrive® for Business. Cloud App Security integrates directly with Office 365 and other services using APIs, maintaining all user functionality without rerouting email traffic or setting up a web proxy.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|String|https://api-eu.tmcas.trendmicro.com|
|API Key||True|Password|*****|
|Verify SSL||False|Boolean|true|


#### Dependencies
| |
|-|
|requests-2.32.4-py3-none-any.whl|
|idna-3.13-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|validators-0.33.0-py3-none-any.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|certifi-2026.4.22-py3-none-any.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|


## Actions
#### Ping
Test connectivity to the Trend Micro CloudApp Security with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Entity Email Search
Search emails based on entities in Trend Micro Cloud App Security. Supported entities: URL, Hash, Email (User entity that matches email address pattern), Email Subject, File Name, IP. Note: only SHA-1 and SHA256 hashes are supported.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Max Days Backwards|Specify how many days backwards to look for emails. Maximum is 90. Default: 30.|False|String|30|
|Max Emails To Return|Specify how many emails to return. Default: 100.|False|String|100|



#### Enrich Entities
Enrich entities with information from Trend Micro Cloud App Security. Supported entities: URL, Hash and Email (User entity that matches email address pattern). Note: action will use the domain part out of the URL during the enrichment.
Timeout - 600 Seconds



#### Mitigate Accounts
Perform mitigation actions on the user account via Trend Micro Cloud App Security. Note: only Exchange accounts are supported.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Mitigation Action|Specify what mitigation action should be applied.|True|List|Disable Account|
|Email Addresses|Specify a comma-separated list of email addresses that need to be mitigated.|True|String||



#### Add Entities To Blocklist
Add entities to a blocklist in Trend Micro Cloud App Security. Supported entities: URL, Hash and Email (User entity that matches email address pattern). Note: only SHA-1 hashes are supported.
Timeout - 600 Seconds



#### Mitigate Emails
Delete or quarantine emails using Trend Micro Cloud App Security. Note: for Gmail you can only delete emails. Note: Currently action only initiates a mitigation, but doesn't check the status of mitigation execution.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Mitigation Action|Specify what mitigation action should be applied.|True|List|Delete|
|Service|Specify the service the is used for emails.|True|List|Gmail|
|Message IDs|Specify a comma-separated list of message ids that need to be mitigated.|True|String||









