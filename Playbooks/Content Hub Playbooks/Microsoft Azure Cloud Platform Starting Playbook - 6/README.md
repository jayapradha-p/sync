# Microsoft Azure Cloud Platform Starting Playbook - 6
Microsoft Azure Cloud Platform Starting Playbook provides reference implementation of how Microsoft Azure Cloud Platform alerts can be processed in Google SecOps.



**Enabled:** False

**Version:** 0

**Type:** Playbook

**Priority:** 3

**Playbook Simulator:** False


### Playbook Trigger
**Trigger Type:** Custom Trigger

**Conditions Operator:** Or

##### Conditions
|Key|Operator|Value|
|---|--------|-----|
|[Event.detection_1_ruleName]|Starts With|ttp_azure|
|[Event.event_target_cloud_environment]|Equals|MICROSOFT_AZURE
|
|[Event.event_metadata_productName]|Contains|Azure|
|[Event.event_metadata_logType]|Equals|OFFICE_365|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|Rule Name Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Change Case Name|The action changes the case's name (title)|Tools|Change Case Name|
|AZURE TAG|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|SUMMARY_DATA reset|The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Case Tag Size|This action includes basic Pythonic string functions as mentioned below - Lower: Converts the input string to lowercase.Upper: Converts the input string to uppercase (duplicated case in the script).Strip: Removes leading and trailing whitespaces from the input string.Title: Converts the first character of each word in the input string to uppercase.Count: Counts the occurrences of `param_1` in the input string.Replace: Replaces occurrences of `param_1` with `param_2` in the input string.Find: Finds the first occurrence of `param_1` in the input string and returns its index.IsAlpha: Checks if all characters in the input string are alphanumeric.IsDigit: Checks if all characters in the input string are digits.Regex Replace: Performs a regex-based replacement of `param_1` with `param_2` in the input string.JSON Serialize: Converts the input string to a JSON formatted string.Regex: Finds all occurrences of the pattern `param_1` in the input string, joins them using `param_2` (defaulting to ", "), and returns the result.DecodeBase64: Decodes the input string from base64 using `param_1` as the encoding type. Default to utf-8EncodeBase64: Encodes the input string in base64 using `param_1` as the encoding type. Default to utf-8RemoveNewLines: Removes new lines from the input string, replacing them with spaces.Split: Splits the input string using `param_1` (or "," if not provided) and adds the result to the Siemplify result.|Functions|String Functions|
|SIEM Get Detection Details|Fetch information about a detection in Google Chronicle.|GoogleChronicle|Get Detection Details|
|Cloud Tag|Add given tag to the case the current alert is grouped to|Siemplify|Case Tag|
|Summary |The action sets a key and value in a specific context (alert or case)|Tools|Set Context Value|
|Close Alert|Closes the current alert|Siemplify|Close Alert|

### Involved Blocks
|Name|Description|
|----|-----------|
|GTI Enrichment|This block enhances case entities with Google Threat Intelligence enrichment information. Works for IPs, URLs, hostnames, domains, hashes (MD5, SHA-1, SHA-256), threat actors, and CVEs.|
|Azure Containment|This block allows the playbook to apply containment actions to Azure user accounts by either updating the password or disabling the account. It also provides the option to ignore the action and take no changes when required.|
|MITRE Enrichment|This block retrieves detailed information about MITRE ATT&CK techniques and their associated mitigations, providing valuable context to understand adversary behaviors and possible defensive actions.|
|Google SecOps Enrichment|This block retrieves relevant details about users and assets involved in the case, enhancing the context available for analysis and subsequent actions within Google SecOps SOAR.|
|Azure Enrichment|This block enriches Siemplify Host and User entities with relevant information from Azure Active Directory, providing additional context to support investigation and response activities.|
|Set Initial Severity|This block sets the initial alert score based on the SIEM detection severity or the rule metadata severity label.|
|Alert Priority|This block sets the alert priority using a previously defined playbook variable, ensuring consistent prioritization logic for the case workflow.|
|High Risk Users Check|This block checks Google GTI sourced alerts against a SOAR custom list to find matches of targeted Industries.|
