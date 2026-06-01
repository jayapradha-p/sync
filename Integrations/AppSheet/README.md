
# AppSheet

AppSheet provides a no-code development platform for application software, which allows users to create mobile, tablet, and web applications using data sources like Google Drive, DropBox, Office 365, and other cloud-based spreadsheet and database platforms.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|String|https://api.appsheet.com|
|App ID||True|String||
|Access Token||True|Password|*****|
|Verify SSL||False|Boolean|true|


#### Dependencies
| |
|-|
|urllib3-2.6.3-py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|certifi-2026.4.22-py3-none-any.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|idna-3.13-py3-none-any.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|


## Actions
#### Delete Record
Delete a record in a table in AppSheet.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Table Name|Specify the JSON object of the record that needs to be deleted. You only need to provide the unique identifier key of the record.|True|String||
|Record JSON Object|Specify the JSON object of the record that needs to be deleted. You only need to provide the "ID" of the record.|True|String||



##### JSON Results
```json
[{"_RowNumber": "61", "Name": "New Park", "State": "IL", "Visited?": "Y", "Location": "44.350000, -68.210000", "Year Established": "2021", "Area (Acres)": "21", "Recreation Visitors (2013)[6]": "", "Image": "", "Photo": "", "Description": "", "Wikipedia URL": ""}]
```



#### Update Record
Update a record in a table in AppSheet.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Table Name|Specify the name of the table in which you want to update a record.|True|String||
|Record JSON Object|Specify the JSON object of the record that needs to be updated. You need to provide the "ID" of the record and fields that you want to update.|True|String||



##### JSON Results
```json
[{"_RowNumber": "61", "Name": "New Park", "State": "IL", "Visited?": "Y", "Location": "44.350000, -68.210000", "Year Established": "2021", "Area (Acres)": "21", "Recreation Visitors (2013)[6]": "", "Image": "", "Photo": "", "Description": "", "Wikipedia URL": ""}]
```



#### Ping
Test connectivity to the AppSheet with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds



#### List Tables
List available tables in an app in AppSheet.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Filter Logic|Specify what filter logic should be applied.|False|List|Equal|
|Filter Value|Specify what value should be used in the filter. If "Equal" is selected, action will try to find the exact match among results and if "Contains" is selected, action will try to find results that contain that substring. If nothing is provided in this parameter, the filter will not be applied. |False|String||
|Max Tables To Return|Specify how many tables to return. Default: 50.|False|String|50|



##### JSON Results
```json
[{"name": "NationalParks", "id": "NationalParks"}]
```



#### Search Records
Search records in a table in AppSheet.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Table Name|Specify the name of the table for which you want to retrieve details.|True|String||
|Selector Query|Specify the selector query, which will be used to limit results. If nothing is provided, action will return all records.|False|String||



##### JSON Results
```json
[{"_RowNumber": "2", "Name": "Acadia", "State": "Maine"}]
```



#### Add Record
Add a record to a table in AppSheet.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Table Name|Specify the JSON object of the record that needs to be updated. You need to provide the unique identifier key and fields that you want to update.|True|String||
|Record JSON Object|Specify the JSON object of the record that needs to be added.|True|String||



##### JSON Results
```json
[{"_RowNumber": "61", "Name": "New Park", "State": "IL", "Visited?": "Y", "Location": "44.350000, -68.210000", "Year Established": "2021", "Area (Acres)": "21", "Recreation Visitors (2013)[6]": "", "Image": "", "Photo": "", "Description": "", "Wikipedia URL": ""}]
```









