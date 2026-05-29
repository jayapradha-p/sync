
# McAfeeMvisionEPO

McAfee MVISION ePO reduces incident response times, strengthens protection, and simplifies risk and security management using automation and end-to-end security visibility. McAfeeÂ® manages the platform infrastructure, upgrades, and maintenance.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|URL|https://api.mvision.mcafee.com|
|Client ID||True|String||
|Client Secret||True|Password|*****|
|Scopes||True|String|epo.device.r, epo.device.w,epo.grps.r, epo.grps.w, epo.sftw.r, epo.tags.r, epo.tags.w|
|Group Name||False|String||
|Verify SSL||False|Boolean|True|


#### Dependencies
| |
|-|
|certifi-2026.4.22-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|idna-3.13-py3-none-any.whl|


## Actions
#### List Tags
List tags that are available in McAfee Mvision ePO.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Max Tags to Return|Specify how many tags to return.|False|String|100|



#### Remove Tag
Remove tag from the endpoint in McAfee Mvision ePO.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Tag Name|Specify what tag  you want to remove from endpoint.|True|String||



#### Enrich Endpoint
Fetch endpoint's system information by its hostname or IP address.
Timeout - 600 Seconds



#### Add Tag
Add tag to the endpoint in McAfee Mvision ePO.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Tag Name|Specify what tag you want to add to endpoint.|True|String||



#### List Endpoints In Group
List endpoints that are in the same group in McAfee Mvision ePO.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Max Endpoints to Return|Specify how many endpoints to return.|False|String|100|
|Group Name|Specify in which groups to search for endpoints|True|String||



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### List Groups
List groups that are available in McAfee Mvision ePO.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Max Groups to Return|Specify how many groups to return.|False|String|100|









