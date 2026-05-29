
# Rapid7InsightIDR

Rapid7's InsightIDR is your security center for incident detection and response, authentication monitoring, and endpoint visibility. InsightIDR identifies unauthorized access from external and internal threats and highlights suspicious activity so you don't have to weed through thousands of data streams.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|String|https://[region].api.insight.rapid7.com|
|API Key||True|Password|*****|
|Verify SSL||False|Boolean|True|


#### Dependencies
| |
|-|
|certifi-2026.4.22-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|EnvironmentCommon-1.0.1-py2.py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|TIPCommon-1.0.12-py2.py3-none-any.whl|
|idna-3.13-py3-none-any.whl|


## Actions
#### Update Investigation
Update investigation in Rapid7 InsightIDR. Note: this action was built using API endpoints that are in preview release.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Investigation ID|Specify the ID of the investigation that needs to be updated.|True|String||
|Status|Specify the status for the investigation.|False|List||
|Disposition|Specify the disposition for the investigation.|False|List||



#### List Investigations
List Rapid7 InsightIDR investigations based on the specified action input parameters.  Note: Action is not working with Siemplify entities, only with action input parameters.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Time Frame|Specify a time frame in hours for which to fetch findings.|False|String|4|
|Record limit|Specify how many records can be returned by the action.|False|String|20|
|Include Closed Investigations?|Specify whether to include closed investigations in results or not.|False|Boolean|false|



#### List Saved Queries
List Rapid7 InsightIDR saved queries.  Note: Action is not working with Siemplify entities, only with action input parameters.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Record limit|Specify how many records can be returned by the action.|False|String|20|



#### Set Investigation Status
Set the status for the specific Rapid7 InsightIDR investigation. Note: Action is not working with Siemplify Entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Investigation ID|ID of investigation to update status for. ID should be in the format like 8ec8e324-4522-4a6e-9838-81496a0cadb0|True|String||
|Status|New Status of investigation.|True|List||



#### Create Saved Query
Create Rapid7 InsightIDR saved query based on the specified action input parameters. Note: Action is not working with Siemplify Entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Name|Name for the new saved query|True|String||
|Statement|A statement to execute in query, should follow LEQL syntax, for example: where(foo=bar)|True|String||
|Time Frame|Specify a time frame in hours for which query should fetch data.|True|String|4|
|Logs|Log names query should execute against. Parameter accepts multiple values as a comma separated string.|False|String||



#### Ping
Test connectivity to the Rapid7 InsightIDR service with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### Set Investigation Assignee
Set the assignee for the specific Rapid7 InsightIDR investigation. Note: Action is not working with Siemplify Entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Investigation ID|ID of investigation to update assignee for. ID should be in the format like 8ec8e324-4522-4a6e-9838-81496a0cadb0.|True|String||
|Assignee email|Email of a new assignee of investigation.|True|String||



#### Run Saved Query
Run a Rapid7 InsightIDR saved query. Note: Action is not working with Siemplify Entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Saved Query ID|Because Saved query names are not unique, provide a saved query ID to execute.|True|String||



#### Delete Saved Query
Delete Rapid7 InsightIDR saved query. Note: Action is not working with Siemplify Entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Saved Query ID|ID of the saved query to delete in the format 00000000-0003-7218-0000-000000000000|True|String||









## Connectors
#### Rapid7 InsightIDR - Investigations Connector
This connector was built using API endpoints that are in preview release. Pull information about investigation from Rapid7 InsightIDR. Note: Dynamic list filter works with the "title" parameter.

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Environment Field Name|Describes the name of the field where the environment name is stored. If the environment field isn't found, the environment is the default environment.|False|String||
|Environment Regex Pattern|A regex pattern to run on the value found in the "Environment Field Name" field. Default is .* to catch all and return the value unchanged. Used to allow the user to manipulate the environment field via regex logic. If the regex pattern is null or empty, or the environment value is null, the final environment result is the default environment.|False|String|.*|
|API Root|API root of the Rapid7 InsightIDR instance.|True|String|https://{instance}.api.insight.rapid7.com|
|API Key|API Key of the Rapid7 InsightIDR account.|True|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Rapid7 InsightIDR server is valid.|False|Boolean|true|
|Sources|Sources that will be used to fetch investigations. Possible values: User, Alert. If nothing is provided, the connector will ingest investigations from both sources.|False|String|ALERT,USER|
|Lowest Priority To Fetch|The lowest priority that needs to be used to fetch investigations. Possible values: Low, Medium, High, Critical. If nothing is specified, the connector ingests alerts with all severities.|False|String|Medium|
|Max Hours Backwards|Number of hours before the first connector iteration to retrieve investigations from. This parameter applies to the initial connector iteration after you enable the connector for the first time, or used as a fallback value in cases where connector's last run timestamp expires.|False|Int|1|
|Max Alerts To Fetch|Number of alerts to process per one connector iteration. Default: 20.|False|Int|20|
|Use dynamic list as a blacklist|If enabled, dynamic lists will be used as a blacklist.|False|Boolean|false|
|Proxy Server Address|The address of the proxy server to use.|False|String||
|Proxy Username|The proxy username to authenticate with.|False|String||
|Proxy Password|The proxy password to authenticate with.|False|Password|*****|




