
# RSANetWitnessEDR

The RSA NetWitness EDR product is an endpoint threat detection solution that exposes malware and other threats, highlights suspicious activity for investigation, and instantly determines the scope of a compromise to help security teams stop advanced threats faster.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root|None|False|None|https://<ip>:9443|
|Username|None|False|String||
|Password|None|False|Password|*****|
|Verify SSL|None|False|Boolean|True|


#### Dependencies
| |
|-|
|chardet-5.2.0-py3-none-any.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|idna-3.8-py3-none-any.whl|
|urllib3-2.2.2-py3-none-any.whl|
|requests-2.32.3-py3-none-any.whl|
|certifi-2024.8.30-py3-none-any.whl|


## Actions
#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Add IP To Blacklist
Add IP To Blacklist in RSA Netwitness EDR.
Timeout - 600 Seconds



##### JSON Results
```json
[{"Ips": ["1.1.1.2", "1.1.1.1"]}]
```



#### Add URL To Blacklist
Add URL To Blacklist in RSA Netwitness EDR.
Timeout - 600 Seconds



##### JSON Results
```json
[{"Domains": ["HTTP://MARKOSXXX.COM/F1Q7QX.PHP", "example.com"]}]
```



#### Enrich Endpoint
Fetch endpoint's system information by its hostname or IP address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|IIOC Score Threshold|Specify IIOC score threshold for the endpoint. If the endpoint exceeds the threshold, the related entity will be marked as suspicious. If nothing is specified, action won’t check the IIOC score.|False|String|50|
|Include IOC Information|If enabled, action will fetch information about the IOCs that are associated with the endpoint|False|Boolean|False|
|Max IOCs To Return|Specify how many IOCs to return. Maximum is 50. This is RSA Netwitness EDR limitation.|False|String|50|



##### JSON Results
```json
[{"Entity": "172.30.xxx.xxxx", "EntityResult": {"Machine": {"DriverErrorCode": "0xe0010014", "ServicePackOS": "0", "MachineStatus": "Offline-DriverError", "Type": "Windows", "VersionInfo": "4.4.0.0", "UserName": "", "OrganizationUnit": "", "LocalIP": "172.30.xxx.xxx", "NetworkSegment": "172.30.xxx.xxx", "Gateway": "172.30.xxx.xxx", "RemoteIP": "172.30.xxx.xxx", "Group": "Default", "AdminStatus": "", "KernelDebuggerDetected": "False", "EarlyStart": "False", "NotifyShutdownModule": "False", "LoadedModuleModule": "False", "NotifyRoutineModule": "False", "UnloadedDriverModule": "False", "ErrorLogModule": "False", "LowLevelReaderModule": "False", "ProcessModule": "False", "WorkerThreadModule": "False", "WindowsHooksModule": "False", "DebuggerAttachedToProcess": "False", "ProcessMonitorModule": "False", "ThreadMonitorModule": "False", "ObjectMonitorModule": "False", "ImageMonitorModule": "False", "DriverMonitorModule": "False", "TdiMonitorModule": "False", "TrackingModule": "False", "TrackingRegistryMonitor": "False", "TrackingObjectMonitor": "False", "TrackingFileMonitor": "False", "TrackingRemoteThreadMonitor": "False", "TrackingCreateProcessMonitor": "False", "TrackingHardLinkMonitor": "False", "TrackingFileBlockMonitor": "False", "TrackingNetworkMonitor": "False", "ECATServerName": "SERVER_NAME", "Online": "False", "IIOCScore": "287", "ChassisType": "Other", "ContainmentSupported": "False", "AgentID": "d96de745-c39b-b513-420d-598952bd463e", "BIOS": "Phoenix Technologies LTD - 6.00 - PhoenixBIOS 4.0 Release 6.0", "OSBuildNumber": "18363", "Comment": "", "ConnectionTime": "9/26/2020 9:12:19 AM", "Language": "en-US", "DNS": "172.30.202.237", "DomainRole": "Member Workstation", "ECATServiceCompileTime": "9/15/2017 10:26:23 PM", "ECATPackageTime": "6/26/2020 6:39:59 AM", "StartTime": "6/29/2020 11:56:36 AM", "ECATDriverCompileTime": "9/15/2017 10:20:48 PM", "DomainName": "xxx.local", "Idle": "False", "IncludedinMonitoring": "True", "IncludedinScanSchedule": "True", "InstallationFailed": "False", "InstallTime": "6/26/2020 6:42:20 AM", "IIOCLevel0": "0", "IIOCLevel1": "2", "IIOCLevel2": "3", "IIOCLevel3": "11", "Country": "USA", "BootTime": "6/29/2020 11:56:31 AM", "LastScan": "9/25/2020 2:26:33 PM", "LastSeen": "9/26/2020 9:24:21 AM", "MAC": "00:50:56:A2:10:9E", "MachineID": "422518b6-54d8-4814-b5d7-02bxxxca0103", "MachineName": "MACHINE_NAME", "AllowAccessDataSourceDomain": "False", "AllowDisplayMixedContent": "False", "AntiVirusDisabled": "False", "BadCertificateWarningDisabled": "False", "CookiesCleanupDisabled": "False", "CrosssiteScriptFilterDisabled": "False", "FirewallDisabled": "False", "IEDepDisabled": "False", "IEEnhancedSecurityDisabled": "False", "IntranetZoneNotificationDisabled": "False", "LUADisabled": "False", "NoAntivirusNotificationDisabled": "False", "NoFirewallNotificationDisabled": "False", "NoUACNotificationDisabled": "False", "NoWindowsUpdateDisabled": "False", "RegistryToolsDisabled": "False", "SmartscreenFilterDisabled": "False", "SystemRestoreDisabled": "False", "TaskManagerDisabled": "False", "UACDisabled": "False", "WarningOnZoneCrossingDisabled": "False", "WarningPostRedirectionDisabled": "False", "Manufacturer": "VMware, Inc.", "Model": "VMware Virtual Platform", "NetworkAdapterPromiscMode": "False", "OperatingSystem": "Microsoft Windows 10 Enterprise Evaluation", "ProcessorArchitecture": "x64", "ProcessorCount": "2", "Platform": "64-bit (x64)", "ProcessorIs32bits": "False", "Processoris64": "True", "ProcessorName": "Intel(R) Xeon(R) CPU E5-2698 v3 @ 2.30GHz", "Scanning": "False", "ScanStartTime": "9/26/2020 9:18:34 AM", "Serial": "VMware-42 22 a8 f8 6a 01 41 ca-12 10 80 75 56 bf 21 4b", "TimeZone": "Pacific Standard Time", "TotalPhysicalMemory": "4294430720", "HTTPSFallbackMode": "False", "BlockingActive": "False", "RoamingAgentsRelaySystemActive": "False", "UserID": "00000000-0000-0000-0000-000000000000", "WindowsDirectory": "C:\\Windows", "NetWitnessInvestigate": "True", "ContainmentStatus": "Not Contained"}, "Iocs": [{"Alertable": "False", "EvaluationDate": "6/26/2020 6:48:13 AM", "IOCContext": "0", "IOCTriggeredOnMachine": "True", "BiasStatus": "Undefined", "Active": "True", "Description": "Network listen", "Type": "Module", "IOCLevel": "3", "LastExecuted": "9/26/2020 9:18:51 AM", "Name": "Network_Listen.sql", "Priority": "5", "Query": "\r\n\r\nSELECT DISTINCT\r\n\t[mp].[FK_Machines] AS [FK_Machines],\r\n\t[mp].[PK_MachineModulePaths] AS [FK_MachineModulePaths]           \r\nFROM\r\n\t[dbo].[MachineModulePaths] AS [mp] WITH(NOLOCK)\r\n\tINNER JOIN [dbo].[MachinesToEvaluate] AS [me] WITH(NOLOCK) ON ([me].[RK_Machines] = [mp].[FK_Machines])\r\nWHERE \r\n\t[mp].[NetworkListen] = 1 AND\r\n\t[mp].[MarkedAsDeleted]  = 0\r\n\r\n", "MachineCount": "1", "ModuleCount": "6"}]}}]
```



#### Get IOC Details
Enrich Siemplify Entities with information about IOCs from RSA Netwitness EDR.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|IOC Level Threshold|Specify IOC level threshold for the entity. If the entity exceeds the threshold, the related entity will be marked as suspicious.|True|List|Medium|



##### JSON Results
```json
[{"Entity": "Autorun_Unsigned_BHO.sql", "EntityResult": {"iocQuery": {"Active": "True", "Alertable": "False", "BlacklistedCount": "0", "GraylistedCount": "0", "Description": "Autorun unsigned BHO", "ErrorMessage": "", "EvaluationMachineCount": "1", "Type": "Windows", "IOCLevel": "2", "LastEvaluationDuration": "0", "LastExecutionDuration": "0", "LastExecuted": "9/26/2020 9:18:51 AM", "MachineCount": "0", "ModuleCount": "0", "Name": "Autorun_Unsigned_BHO.sql", "Persistent": "True", "Priority": "5", "Query": "\r\n\r\nSELECT DISTINCT\r\n\t[mp].[FK_Machines] AS [FK_Machines],\r\n\t[mp].[PK_MachineModulePaths] AS [FK_MachineModulePaths]\r\nFROM\r\n\t[dbo].[mocAutoruns] AS [ar] WITH(NOLOCK)\r\n\tINNER JOIN [dbo].[MachinesToEvaluate] AS [me] WITH(NOLOCK) ON ([me].[RK_Machines] = [ar].[FK_Machines])\r\n\tINNER JOIN [dbo].[Paths] AS [pa] WITH(NOLOCK) ON ([pa].[PK_Paths] = [ar].[FK_Paths__RegistryPath])\r\n\tINNER JOIN [dbo].[MachineModulePaths] AS [mp] WITH(NOLOCK) ON ([mp].[PK_MachineModulePaths] = [ar].[FK_MachineModulePaths] AND [mp].[FK_Machines] = [ar].[FK_Machines])\r\n\tINNER JOIN [dbo].[Modules] AS [mo] WITH(NOLOCK) ON ([mo].[PK_Modules] = [mp].[FK_Modules])\r\nWHERE \r\n\t[ar].[Type] = 5 AND\r\n\t[pa].[Path] LIKE N'%\\SOFTWARE%Microsoft\\Windows\\CurrentVersion\\Explorer\\Browser Helper Objects\\%' AND\r\n\t[mo].[ModuleSignaturePresent] = 0 AND\r\n\t[ar].[MarkedAsDeleted] = 0\r\n\r\n", "UserDefined": "False", "WhitelistedCount": "0"}}}]
```









