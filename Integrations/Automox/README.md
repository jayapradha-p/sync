
# Automox

Automox is the modern, cloud-native endpoint-hardening platform that empowers organizations to remediate vulnerabilities faster than they can be weaponized.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|API root of the Automox instance.|True|String|https://{{api_root}}|
|API Key|API key of the Automox instance.|True|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Automox is valid.|False|Boolean|true|


#### Dependencies
| |
|-|
|urllib3-2.2.3-py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|TIPCommon-1.0.12-py2.py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|
|chardet-5.2.0-py3-none-any.whl|
|idna-3.10-py3-none-any.whl|
|certifi-2024.8.30-py3-none-any.whl|


## Actions
#### Execute Policy
Execute a policy in Automox. Supported entities: Hostname, IP Address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Remediation Scope|Specify the remediation scope for the action. If “Only Entities” is selected, then action will execute policies only on the valid entities in the scope. If “All Devices” is selected, then action will execute the policy on all devices in the organization.|True|List|All Devices|
|Policy Name|Specify the name of the policy that needs to be executed.|True|String||



#### List Policies
List available policies in Automox.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Filter Key|Specify the key that needs to be used to filter policy.|False|List|Select One|
|Filter Logic|Specify what filter logic should be applied. Filtering logic is working based on the value  provided in the “Filter Key” parameter.|False|List|Not Specified|
|Filter Value|Specify what value should be used in the filter. If “Equal“ is selected, action will try to find the exact match among results and if “Contains“ is selected, action will try to find results that contain that substring. If nothing is provided in this parameter, the filter will not be applied. Filtering logic is working based on the value  provided in the “Filter Key” parameter.|False|String||
|Max Records To Return|Specify how many records to return. If nothing is provided, action will return 50 records.|False|String|50|



#### Ping
Test connectivity to the Automox with parameters provided at the integration configuration page on the Marketplace tab
Timeout - 600 Seconds



#### Execute Device Command
Execute a command on the endpoint in Automox. Supported entities: Hostname, IP Address. Note: Action is running as async, please adjust script timeout value in Chronicle SOAR for action as needed.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Command|Specify a command that needs to be executed on the device. Note: if "Install Specific Patches" is provided, parameter "Patch Names" is mandatory.|False|List|Scan Device|
|Patch Names|Specify a comma-separated list of patches that need to be installed.|False|String||



#### Enrich Entities
Enrich entities using information from Automox. Supported entities: Hostname, IP Address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Return Patches|If enabled, action will return a list of patches that need to be updated on the machine. Note: action will not return patches that were installed or the ones that are currently ignored.|False|Boolean|true|
|Max Patches To Return|Specify how many patches to return. If nothing is provided, action will return 50 patches.|False|String|50|









