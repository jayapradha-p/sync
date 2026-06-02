
# ReversinglabsA1000

The A1000 Malware Analysis Platform supports advanced hunting and investigations through high-speed automated static analysis.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Api Root||True|String|https://a1000.reversinglabs.com|
|Username||True|String||
|Password||True|Password|*****|


#### Dependencies
| |
|-|
|urllib3-2.6.3-py3-none-any.whl|
|charset_normalizer-3.4.6-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|idna-3.11-py3-none-any.whl|
|requests-2.32.5-py3-none-any.whl|
|certifi-2026.2.25-py3-none-any.whl|


## Actions
#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Delete Sample
Delete a set of samples that exist on the A1000 appliance. All related data, including extracted samples and metadata, will be deleted
Timeout - 600 Seconds



#### Get Scan Status
 Return the processing status in the A1000 system for the list of hash values
Timeout - 600 Seconds



#### Upload File
Upload a file for analysis on the A1000 appliance
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|File Path|Target file path.|True|String||



#### Get Report
Get a summary classification report and all details for a sample or a list of samples using hash value(s)
Timeout - 600 Seconds









