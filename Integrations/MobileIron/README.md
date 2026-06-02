
# MobileIron

MobileIron's mobile device management (MDM) capabilities give you the fundamental visibility and IT controls needed to secure, manage, and monitor any corporate- or employee-owned mobile device or desktop that accesses business critical data.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|URL|https://x.x.x.x/|
|Username||True|String||
|Password||True|Password|*****|
|Admin Device ID||True|Int|1|
|Cloud Instance||False|Boolean||
|Verify SSL||False|Boolean||


#### Dependencies
| |
|-|
|urllib3-2.6.3-py3-none-any.whl|
|charset_normalizer-3.4.6-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|idna-3.11-py3-none-any.whl|
|requests-2.32.5-py3-none-any.whl|
|certifi-2026.2.25-py3-none-any.whl|


## Actions
#### List Devices
Get the list of al the devices at the system.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Fields To Fetch|The values of the inserted fields will be fetched for a device(Has to be comma separated string), ex: ios.DeviceName,user.display_name,user.email_address,user.user_id|False|String||



#### Ping
Test integration connectiovity.
Timeout - 600 Seconds



#### Unlock Device by UUID
Unlock device by it's UUID.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Device UUID|The UUID of the target device.|True|String||



#### Fetch System Information
Fetch system information for device by it's IP adddress.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Fields To Fetch|The values of the inserted fields will be fetched for a device(Has to be comma separated string), ex: ios.DeviceName,user.display_name,user.email_address,user.user_id|False|String||



#### Fetch System Information By UUID
Get device system information by it's UID.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Device UUID|The UUID of the target device.|True|String||



#### Unlock Device
Ulock device by it's IP address.
Timeout - 600 Seconds









