# GCP Instance Containment - 1
This block stops running GCP Compute VM instances, shutting them down gracefully and allowing them to be restarted later if needed. It uses a boolean input to control manual or automatic execution and returns the containment result, false on failure, or an empty value if no action is taken.



**Enabled:** True

**Version:** 0

**Type:** Block

**Priority:** 2

**Playbook Simulator:** False


##### Input Parameters
|Name|Default Value|
|----|-------------|
|Manual|Yes|


### Involved Steps (Unordered)
|Step Name|Description|Integration|Original Action|
|---------|-----------|-----------|---------------|
|Count Hostnames|Count the number of entities from a specific scope.|SiemplifyUtilities|Count Entities In Scope|
|Stop Instance Auto|Stops a running instance, shutting it down cleanly, and allows you to restart the instance at a later time. Stopped instances do not incur VM usage charges while they are stopped. However, resources that the VM is using, such as persistent disks and static IP addresses, will continue to be charged until they are deleted.|GoogleCloudCompute|Stop Instance|
|Stop Instance|Stops a running instance, shutting it down cleanly, and allows you to restart the instance at a later time. Stopped instances do not incur VM usage charges while they are stopped. However, resources that the VM is using, such as persistent disks and static IP addresses, will continue to be charged until they are deleted.|GoogleCloudCompute|Stop Instance|
|List Instances|List Google Cloud Compute instances based on the specified search criteria. Note that action is not working on Siemplify entities.|GoogleCloudCompute|List Instances|

