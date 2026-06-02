
# AtlassianConfluenceServer

Confluence is a collaboration tool that brings people, knowledge, and ideas together in a shared workspace, so you can do your best work with the confidence of your entire organization's expertise behind you. This integration is working with the server deployment option (self hosted).

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root|Specify Confluence Server Api Root to connect to.|True|String|https://{confluence_server_ip}:{port}|
|Username|Specify a username to use for connection. Integration supports authentication on either username+password or personal access token (PAT). Please refer to the documentation for instructions.|False|String|None|
|Password|Specify a password to use for connection. Integration supports authentication on either username+password or personal access token (PAT). Please refer to the documentation for instructions.|False|Password|*****|
|Api Token|Specify a token to use for connection. Integration supports authentication on either username+password or personal access token (PAT). Please refer to the documentation for instructions.|False|Password|*****|
|Verify SSL|If enabled, the certificate configured for the API root is validated.|False|Boolean|true|


#### Dependencies
| |
|-|
|TIPCommon-1.0.14-py2.py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|
|chardet-5.2.0-py3-none-any.whl|
|idna-3.8-py3-none-any.whl|
|certifi-2024.8.30-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|


## Actions
#### Get Page by ID
Get Atlassian Confluence Server page by id. Note: This action doesn’t run on Chronicle SOAR entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Page ID|Specify the page id to return.|True|String||
|Expand|Specify the expand parameter to return additional information about the page. Parameter accepts multiple values as a comma separated list. By default with body.storage the content of the page is fetched.|False|String|body.storage|



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Get Child Pages
Get child pages for the Atlassian Confluence Server page. Note: This action doesn’t run on Chronicle SOAR entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Page ID|Specify the page id to return.|True|String||
|Max Records to Return|Specify the limit of child pages to return.|True|String|10|



#### List Pages
List pages available in the Atlassian Confluence Server instance based on provided criteria. Note: This action doesn’t run on Chronicle SOAR entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Filter Key|Specify the key that needs to be used to filter pages.|False|List|Select One|
|Filter Logic|Specify what filter logic should be applied. Filtering logic is working based on the value  provided in the “Filter Key” parameter.|False|List|Not Specified|
|Filter Value|Specify what value should be used in the filter. If “Equal“ is selected, action will try to find the exact match among results and if “Contains“ is selected, action will try to find results that contain that substring. If nothing is provided in this parameter, the filter will not be applied. Filtering logic is working based on the value  provided in the “Filter Key” parameter.|False|String||
|Max Records to Return|Specify how many records to return. If nothing is provided, action will return 50 records.|False|String|50|



#### Get Page Comments
Get comments for the Atlassian Confluence Server page. Note: This action doesn’t run on Chronicle SOAR entities.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Page ID|Specify the page id to return.|True|String||
|Expand|Specify the expand parameter to return additional information about the page. Parameter accepts multiple values as a comma separated list. By default with body.storage the content of the page is fetched.|False|String|body.storage|
|Max Records to Return|Specify the limit of child pages to return.|True|String|10|









