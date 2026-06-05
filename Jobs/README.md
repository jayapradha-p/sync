## CA Close Ticket In CA For Closed Case - 3
Sync closure of the tickets at the CA Desk Manager with Siemplify cases closure.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String|False|http://x.x.x.x:<port>|
|Username|String|False|dsdsdsds|
|Password|String|False|sddssds|
|Group Filter|String|False|Test|
|Group Field|String|False|group.combo_name|
|Ticket Final Status|String|False|Closed|
|Script Name|String|False|TEST CLOSE|

## Google Chronicle Alerts Creator Job - 1
This job will sync new SOAR alerts with Chronicle SIEM.
Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment|String|False|Default Environment|
|API Root|String|False|https://backstory.googleapis.com|
|Verify SSL|Boolean|False|true|
|User's Service Account|Password|False|*****|
|Workload Identity Email|Password|False|*****|

## Google Chronicle Alerts Creator Job - 13
This job will sync new SOAR alerts with Chronicle SIEM.
Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment|String|False|Default Environment|
|API Root|String|False|https://backstory.googleapis.com|
|Verify SSL|Boolean|False|true|
|User's Service Account|Password|False|*****|
|Workload Identity Email|Password|False|*****|

## Google Chronicle Alerts Creator Job - 5
This job will sync new SOAR alerts with Chronicle SIEM.
Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment|String|False|Default Environment|
|API Root|String|False|https://backstory.googleapis.com|
|Verify SSL|Boolean|False|false|
|User's Service Account|Password|False|*****|
|Workload Identity Email|Password|False|*****|

## Google Chronicle Sync Job - 1
This job will synchronize information about Chronicle SOAR Cases and Chronicle SOAR Alerts with Chronicle SIEM.
 Note: This job is only supported from Chronicle SOAR version 6.1.44 and higher.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment|String|False|Default Environment|
|API Root|String|False|https://backstory.googleapis.com|
|Max Hours Backwards|String|False|24|
|Verify SSL|Boolean|False|true|
|User's Service Account|Password|False|*****|
|Workload Identity Email|Password|False|*****|

## Google Chronicle Sync Job - 2
This job will synchronize information about Chronicle SOAR Cases and Chronicle SOAR Alerts with Chronicle SIEM.
 Note: This job is only supported from Chronicle SOAR version 6.1.44 and higher.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment|String|False|Default Environment|
|API Root|String|False|https://backstory.googleapis.com|
|Max Hours Backwards|String|False|24|
|Verify SSL|Boolean|False|false|
|User's Service Account|Password|False|*****|
|Workload Identity Email|Password|False|*****|

## Google Chronicle Sync Job -21
This job will synchronize information about Chronicle SOAR Cases and Chronicle SOAR Alerts with Chronicle SIEM.
 Note: This job is only supported from Chronicle SOAR version 6.1.44 and higher.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment|String|False|Default Environment|
|API Root|String|False|https://backstory.googleapis.com|
|Max Hours Backwards|String|False|24|
|Verify SSL|Boolean|False|true|
|User's Service Account|Password|False|*****|
|Workload Identity Email|Password|False|*****|

## Refresh Token Renewal Job - 1
Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Integration Environments|String|False|jhjhjh|
|Connector Names|String|False|m,nmnmnnm|

## Refresh Token Renewal Job - 4
Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Integration Environments|String|False|sddssdsd|

## Refresh Token Renewal Job - 8
Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Integration Environments|String|False|dssdsdsdsd|
|Connector Names|String|False|dsd|

## Refresh Token Renewal Job
Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Integration Environments|String|False|dsddss|
|Connector Names|String|False|dsdsdds|

## Service Sync Closed Incidents
This job will synchronize closed ServiceNow incidents and Google SecOps alerts. This job works with ServiceNow incidents that were ingested as alerts and also cases, which contains tag “ServiceNow” and “TICKET_ID” context value with Incident Number inside of it.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Api Root|String|False|https://{dev-instance}.service-now.com/api/now/v1/|
|Username|String|False|dsdssdds|
|Verify SSL|Boolean|False|true|
|Client ID|String|False|sdssddsds|
|Use Oauth Authentication|Boolean|False|false|
|Max Hours Backwards|Int|False|24|
|Table Name|String|False|ddssdsd|
|Password|Password|False|*****|
|Client Secret|Password|False|*****|
|Refresh Token|Password|False|*****|

## Sync Alerts - 1
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|https://api.crowdstrike.com|
|Client ID|String|False|kjhjkkjkj|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|true|
|Client Secret|Password|False|*****|

## Sync Alerts - 10
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|https://api.crowdstrike.com|
|Client ID|String|False|ssdsdssd|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|false|
|Client Secret|Password|False|*****|

## Sync Alerts - 12
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|https://api.crowdstrike.com|
|Client ID|String|False|dssdsdds|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|true|
|Client Secret|Password|False|*****|

## Sync Alerts - 15
This job will synchronize Google SecOps Alerts and SentinelOne alerts. The job synchronizes status. Requires “SentinelOne Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” you will need to add an “Alert_ID” Alert Context Value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|dssdsddsd|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|true|
|API Token|Password|False|*****|

## Sync Alerts - 16
This job will synchronize Google SecOps Alerts and SentinelOne alerts. The job synchronizes status. Requires “SentinelOne Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” you will need to add an “Alert_ID” Alert Context Value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|sdssdds|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|false|
|API Token|Password|False|*****|

## Sync Alerts - 17
This job will synchronize Google SecOps Alerts and SentinelOne alerts. The job synchronizes status. Requires “SentinelOne Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” you will need to add an “Alert_ID” Alert Context Value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|cxcxcx|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|true|
|API Token|Password|False|*****|

## Sync Alerts - 22d
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|https://api.crowdstrike.com|
|Client ID|String|False|ssddsdssd|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|true|
|Client Secret|Password|False|*****|

## Sync Alerts - 3
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|https://api.crowdstrike.com|
|Client ID|String|False|ssdsssd|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|false|
|Client Secret|Password|False|*****|

## Sync Alerts - 4
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|https://api.crowdstrike.com|
|Client ID|String|False|sddssd|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|true|
|Client Secret|Password|False|*****|

## Sync Alerts - 5
This job will synchronize Google SecOps Alerts and SentinelOne alerts. The job synchronizes status. Requires “SentinelOne Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” you will need to add an “Alert_ID” Alert Context Value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|ssdssd|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|true|
|API Token|Password|False|*****|

## Sync Alerts - 6
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|https://api.crowdstrike.com|
|Client ID|String|False|sdssddsds|
|Max Hours Backwards|Int|False|24|
|Client Secret|Password|False|*****|
|Verify SSL|Boolean|False|false|

## Sync Alerts - 8
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|https://api.crowdstrike.com|
|Client ID|String|False|qwewwewwe|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|false|
|Client Secret|Password|False|*****|

## Sync Alerts - 9
This job will synchronize Google SecOps Alerts and SentinelOne alerts. The job synchronizes status. Requires “SentinelOne Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” you will need to add an “Alert_ID” Alert Context Value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|sdsddssdsd|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|false|
|API Token|Password|False|*****|

## Sync Alerts
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|https://api.crowdstrike.com|
|Client ID|String|False|ssdsdasd|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|true|
|Client Secret|Password|False|*****|

## Sync Closed Incidents - jaya
This job will synchronize closed ServiceNow incidents and Google SecOps alerts. This job works with ServiceNow incidents that were ingested as alerts and also cases, which contains tag “ServiceNow” and “TICKET_ID” context value with Incident Number inside of it.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Api Root|String|False|https://{dev-instance}.service-now.com/api/now/v1/|
|Username|String|False|jhjhjhjjkkjkjjk|
|Password|Password|False|*****|
|Verify SSL|Boolean|False|true|
|Client ID|String|False|jhhjjh|
|Client Secret|Password|False|*****|
|Refresh Token|Password|False|*****|
|Use Oauth Authentication|Boolean|False|false|
|Max Hours Backwards|Int|False|24|
|Table Name|String|False|jkjkkjkj|

## Sync Closure
Close tickets in Jira if corresponding Google SecOps alerts were closed.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String|False|https://{jira_address}|
|Username|String|False|sdsdds|
|Environment|String|False||
|Project Names|String|False|project names separated by comma|
|Days Backwards|String|False|1|
|API Token|Password|False|*****|

## Sync Comments - 19
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String|False|http://x.x.x.x:<port>|
|Username|String|False|sdssddssd|
|Summery Field|String|False|summery.combo_name|
|Ticket Fields|String|False|summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String|False|Test|
|Ticket Type Field|Boolean|False|true|
|Analyst Type Field|Boolean|False|true|
|Time Stamp Field|Boolean|False|true|
|Timezone String|Boolean|False|true|
|Password|Password|False|*****|

## Sync Comments - 2
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String|False|http://x.x.x.x:<port>|
|Username|String|False|tyyuu|
|Summery Field|String|False|summery.combo_name|
|Ticket Fields|String|False|summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String|False|Test|
|Ticket Type Field|Boolean|False|true|
|Analyst Type Field|Boolean|False|true|
|Time Stamp Field|Boolean|False|true|
|Timezone String|Boolean|False|true|
|Password|Password|False|*****|

## Sync Comments - 3
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Analyst Type Field|Boolean|False|true|
|Time Stamp Field|Boolean|False|true|
|Timezone String|Boolean|False|true|
|API Root|String|False|http://x.x.x.x:<port>|
|Username|String|False|dsdsds|
|Summery Field|String|False|summery.combo_name|
|Ticket Fields|String|False|summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String|False|Test|
|Ticket Type Field|Boolean|False|true|
|Password|Password|False|*****|

## Sync Comments - 4
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String|False|http://x.x.x.x:<port>|
|Username|String|False|dsdsds|
|Summery Field|String|False|summery.combo_name|
|Ticket Fields|String|False|summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String|False|Test|
|Ticket Type Field|Boolean|False|true|
|Analyst Type Field|Boolean|False|true|
|Time Stamp Field|Boolean|False|true|
|Timezone String|Boolean|False|true|
|Password|Password|False|*****|

## Sync Comments - 5
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String|False|http://x.x.x.x:<port>|
|Username|String|False|ssdsddssd|
|Summery Field|String|False|summery.combo_name|
|Ticket Fields|String|False|summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String|False|Test|
|Ticket Type Field|Boolean|False|true|
|Analyst Type Field|Boolean|False|true|
|Time Stamp Field|Boolean|False|true|
|Timezone String|Boolean|False|true|
|Password|Password|False|*****|

## Sync Comments - 6
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String|False|http://x.x.x.x:<port>|
|Username|String|False|hghjjkhjh|
|Summery Field|String|False|summery.combo_name|
|Ticket Fields|String|False|summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String|False|Test|
|Ticket Type Field|Boolean|False|true|
|Analyst Type Field|Boolean|False|true|
|Time Stamp Field|Boolean|False|true|
|Timezone String|Boolean|False|true|
|Password|Password|False|*****|

## Sync Comments - 7
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String|False|http://x.x.x.x:<port>|
|Username|String|False|ddsdssdsd|
|Summery Field|String|False|summery.combo_name|
|Ticket Fields|String|False|summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String|False|Test|
|Ticket Type Field|Boolean|False|true|
|Analyst Type Field|Boolean|False|true|
|Time Stamp Field|Boolean|False|true|
|Timezone String|Boolean|False|true|
|Password|Password|False|*****|

## Sync Comments - 8
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String|False|http://x.x.x.x:<port>|
|Username|String|False|dedfdffddf|
|Summery Field|String|False|summery.combo_name|
|Ticket Fields|String|False|summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String|False|Test|
|Ticket Type Field|Boolean|False|true|
|Analyst Type Field|Boolean|False|true|
|Time Stamp Field|Boolean|False|true|
|Timezone String|Boolean|False|true|
|Password|Password|False|*****|

## Sync Comments
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String|False|http://x.x.x.x:<port>|
|Username|String|False|jj,skskjkj|
|Summery Field|String|False|summery.combo_name|
|Ticket Fields|String|False|summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String|False|Test|
|Ticket Type Field|Boolean|False|true|
|Analyst Type Field|Boolean|False|true|
|Time Stamp Field|Boolean|False|true|
|Timezone String|Boolean|False|true|
|Password|Password|False|*****|

## Sync Incidents - 11
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|Api Root|String|False||
|Api Key ID|String|False|sdssdsdsdsd|
|Max Hours Backwards|Int|False|24|
|User Mapping JSON|String|False|{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean|False|true|
|Api Key|Password|False|*****|

## Sync Incidents - 111
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|Api Root|String|False||
|Api Key ID|String|False|kjjkkjkj|
|Max Hours Backwards|Int|False|24|
|User Mapping JSON|String|False|{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean|False|true|
|Api Key|Password|False|*****|

## Sync Incidents - 1s
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|Api Root|String|False||
|Api Key ID|String|False|ss|
|Max Hours Backwards|Int|False|24|
|User Mapping JSON|String|False|{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean|False|true|
|Api Key|Password|False|*****|

## Sync Incidents - 2
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|Api Root|String|False|dssdsdsdsd|
|Api Key ID|String|False|dsdssdsd|
|Max Hours Backwards|Int|False|24|
|User Mapping JSON|String|False|{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean|False|false|
|Api Key|Password|False|*****|

## Sync Incidents - 22
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|Api Root|String|False|cxcxcxc|
|Api Key ID|String|False|sds|
|Max Hours Backwards|Int|False|24|
|User Mapping JSON|String|False|{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean|False|true|
|Api Key|Password|False|*****|

## Sync Incidents - 3
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|Api Root|String|False||
|Api Key ID|String|False|dssdsdsd|
|Max Hours Backwards|Int|False|24|
|User Mapping JSON|String|False|{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean|False|true|
|Api Key|Password|False|*****|

## Sync Incidents - 7
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|Api Root|String|False|ssddsddsds|
|Api Key ID|String|False|dssdsd|
|Max Hours Backwards|Int|False|24|
|User Mapping JSON|String|False|{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean|False|false|
|Api Key|Password|False|*****|

## Sync Incidents V2 - 20
Use the Sync Incidents V2 job to synchronize Google SecOps alerts with Microsoft Sentinel incidents. This job ensures that comments, statuses, and tags are synchronized bi-directionally between both systems. Note: Assignee and severity synchronization occurs exclusively from Microsoft Sentinel to Google SecOps. For the job to identify the correct information, the Google SecOps case must have the Microsoft Sentinel Incident tag. This job only works on alerts from the Microsoft Azure Sentinel Incident Connector v2.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|Azure Subscription ID|String|False|sddssd|
|Azure Active Directory ID|String|False|dssdsdsds|
|OAUTH2 Login Endpoint Url|String|False|https://login.microsoftonline.com|
|Management API Root|String|False|https://msdanagement.azure.com|
|Azure Resource Group|String|False|sdsdsds|
|Azure Sentinel Workspace Name|String|False|dssd|
|Client ID|String|False|dsdsdsdsdds|
|Max Hours Backwards|Int|False|24|
|Sync Assignee|Boolean|False|false|
|Verify SSL|Boolean|False|true|
|Client Secret|Password|False|*****|

## Sync Incidents
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|Api Root|String|False||
|Api Key ID|String|False|54|
|Max Hours Backwards|Int|False|24|
|User Mapping JSON|String|False|{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean|False|false|
|Api Key|Password|False|*****|

## Sync Threats - 18
This job will synchronize Google SecOps Alerts and SentinelOne threats. The job synchronizes comments and status. Requires “SentinelOne Threat” tag on the case. Note: If the alert didn’t originate from “Threats Connector” you will need to add an “Threat_ID” Alert Context Value for the job to be able to find the correct information. 


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|dsdsd|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|true|
|API Token|Password|False|*****|

## Sync Threats - 5
This job will synchronize Google SecOps Alerts and SentinelOne threats. The job synchronizes comments and status. Requires “SentinelOne Threat” tag on the case. Note: If the alert didn’t originate from “Threats Connector” you will need to add an “Threat_ID” Alert Context Value for the job to be able to find the correct information. 


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|fddfdfdf|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|false|
|API Token|Password|False|*****|

## Sync Threats - 8
This job will synchronize Google SecOps Alerts and SentinelOne threats. The job synchronizes comments and status. Requires “SentinelOne Threat” tag on the case. Note: If the alert didn’t originate from “Threats Connector” you will need to add an “Threat_ID” Alert Context Value for the job to be able to find the correct information. 


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|dssddfdf|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|false|
|API Token|Password|False|*****|

## Sync Threats
This job will synchronize Google SecOps Alerts and SentinelOne threats. The job synchronizes comments and status. Requires “SentinelOne Threat” tag on the case. Note: If the alert didn’t originate from “Threats Connector” you will need to add an “Threat_ID” Alert Context Value for the job to be able to find the correct information. 


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String|False|Default Environment|
|API Root|String|False|ssssdsd|
|Max Hours Backwards|Int|False|24|
|Verify SSL|Boolean|False|false|
|API Token|Password|False|*****|

## Token Renewal Job - 2
Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Integration Environments|String|False|hello|
|Connector Names|String|False|hello|

## Token Renewal Job - 4
Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Integration Environments|String|False|dssddssdds|
|Connector Names|String|False|sddssd|

## Token Renewal Job
Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Integration Environments|String|False|jkhhjkhjk|
|Connector Names|String|False||

## jira new Sync Closure
Close tickets in Jira if corresponding Google SecOps alerts were closed.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String|False|https://{jira_address}|
|Username|String|False||
|Environment|String|False||
|Project Names|String|False|project names separated by comma|
|Days Backwards|String|False|1|
|API Token|Password|False|*****|

