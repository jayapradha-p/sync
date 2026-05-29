
# Snowflake

Snowflake enables data storage, processing, and analytic solutions that are faster, easier to use, and far more flexible than traditional offerings. Snowflake combines a completely new SQL query engine with an innovative architecture natively designed for the cloud. To the user, Snowflake provides all of the functionality of an enterprise analytic database, along with many additional special features and unique capabilities.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|API root of the Snowflake instance.|True|String|https://{your_instance}.snowflakecomputing.com|
|Account|The name of the account configured with Snowflake.|True|String||
|Username|Username used to access Snowflake.|True|String||
|Private Key|Private key that is used for authentication.|True|Password|*****|
|Verify SSL|If enabled, verify the SSL certificate for the connection to the Snowflake server is valid.|False|Boolean|True|


#### Dependencies
| |
|-|
|chardet-5.2.0-py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|idna-3.8-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|
|TIPCommon-1.0.11-py2.py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|
|PyJWT-2.9.0-py3-none-any.whl|
|certifi-2024.8.30-py3-none-any.whl|


## Actions
#### Execute Simple Query
Execute a query based on parameters in Snowflake. Note: Action is running as async, please adjust script timeout value in Siemplify IDE for action as needed.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Database|Specify the name of the database in which you want to execute the query.|True|String||
|Table|Specify the name of the table in which you want to execute the query.|True|String||
|Schema|Specify the name of the schema in which you want to execute the query.|False|String||
|Where Filter|Specify the WHERE filter for the query  that needs to be executed. Note: you don't need to limit and sort. Also, you don’t need to provide WHERE string in the payload. Only single quotes are supported in the query.|False|String||
|Fields To Return|Specify what fields to return. If nothing is provided action will return all fields. Wildcard character is supported.|False|String|*|
|Sort Field|Specify what parameter should be used for sorting.|False|String||
|Sort Order|Specify the order of sorting.|False|List|ASC|
|Max Results To Return|Specify how many results to return. Default: 50.|False|String|50|



#### Execute Custom Query
Execute a custom query in Snowflake. Note: Action is running as async, please adjust script timeout value in Siemplify IDE for action as needed.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Query|Specify the query that needs to be executed in Snowflake. Note: query shouldn't contain LIMIT keyword, because it’s added automatically. Only single quotes are supported in the query.|True|String||
|Database|Specify the name of the database in which you want to execute the query.|True|String||
|Schema|Specify the name of the schema in which you want to execute the query.|False|String||
|Max Results To Return|Specify how many results to return for the query. Default: 50.|False|String|50|



#### Ping
Test connectivity to the Snowflake with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds









