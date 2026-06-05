## CA Close Ticket In CA For Closed Case - 3
Sync closure of the tickets at the CA Desk Manager with Siemplify cases closure.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String||http://x.x.x.x:<port>|
|Username|String||dsdsdsds|
|Password|String||sddssds|
|Group Filter|String||Test|
|Group Field|String||group.combo_name|
|Ticket Final Status|String||Closed|
|Script Name|String||TEST CLOSE|

## Google Chronicle Alerts Creator Job - 1
This job will sync new SOAR alerts with Chronicle SIEM.
Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment|String||Default Environment|
|API Root|String||https://backstory.googleapis.com|
|Verify SSL|Boolean||true|
|User's Service Account|Password||*****|
|Workload Identity Email|Password||*****|

## Google Chronicle Alerts Creator Job - 13
This job will sync new SOAR alerts with Chronicle SIEM.
Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment|String||Default Environment|
|API Root|String||https://backstory.googleapis.com|
|Verify SSL|Boolean||true|
|User's Service Account|Password||*****|
|Workload Identity Email|Password||*****|

## Google Chronicle Alerts Creator Job - 5
This job will sync new SOAR alerts with Chronicle SIEM.
Note: This job is only supported from Chronicle SOAR version 6.2.30 and higher.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment|String||Default Environment|
|API Root|String||https://backstory.googleapis.com|
|Verify SSL|Boolean||false|
|User's Service Account|Password||*****|
|Workload Identity Email|Password||*****|

## Google Chronicle Sync Job - 1
This job will synchronize information about Chronicle SOAR Cases and Chronicle SOAR Alerts with Chronicle SIEM.
 Note: This job is only supported from Chronicle SOAR version 6.1.44 and higher.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment|String||Default Environment|
|API Root|String||https://backstory.googleapis.com|
|Max Hours Backwards|String||24|
|Verify SSL|Boolean||true|
|User's Service Account|Password||*****|
|Workload Identity Email|Password||*****|

## Google Chronicle Sync Job - 2
This job will synchronize information about Chronicle SOAR Cases and Chronicle SOAR Alerts with Chronicle SIEM.
 Note: This job is only supported from Chronicle SOAR version 6.1.44 and higher.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment|String||Default Environment|
|API Root|String||https://backstory.googleapis.com|
|Max Hours Backwards|String||24|
|Verify SSL|Boolean||false|
|User's Service Account|Password||*****|
|Workload Identity Email|Password||*****|

## Google Chronicle Sync Job -21
This job will synchronize information about Chronicle SOAR Cases and Chronicle SOAR Alerts with Chronicle SIEM.
 Note: This job is only supported from Chronicle SOAR version 6.1.44 and higher.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment|String||Default Environment|
|API Root|String||https://backstory.googleapis.com|
|Max Hours Backwards|String||24|
|Verify SSL|Boolean||true|
|User's Service Account|Password||*****|
|Workload Identity Email|Password||*****|

## Refresh Token Renewal Job - 1
Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Integration Environments|String||jhjhjh|
|Connector Names|String||m,nmnmnnm|

## Refresh Token Renewal Job - 4
Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Integration Environments|String||sddssdsd|

## Refresh Token Renewal Job - 8
Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Integration Environments|String||dssdsdsdsd|
|Connector Names|String||dsd|

## Refresh Token Renewal Job
Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Integration Environments|String||dsddss|
|Connector Names|String||dsdsdds|

## Service Sync Closed Incidents
This job will synchronize closed ServiceNow incidents and Google SecOps alerts. This job works with ServiceNow incidents that were ingested as alerts and also cases, which contains tag “ServiceNow” and “TICKET_ID” context value with Incident Number inside of it.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Api Root|String||https://{dev-instance}.service-now.com/api/now/v1/|
|Username|String||dsdssdds|
|Verify SSL|Boolean||true|
|Client ID|String||sdssddsds|
|Use Oauth Authentication|Boolean||false|
|Max Hours Backwards|Int||24|
|Table Name|String||ddssdsd|
|Password|Password||*****|
|Client Secret|Password||*****|
|Refresh Token|Password||*****|

## Sync Alerts - 1
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||https://api.crowdstrike.com|
|Client ID|String||kjhjkkjkj|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||true|
|Client Secret|Password||*****|

## Sync Alerts - 10
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||https://api.crowdstrike.com|
|Client ID|String||ssdsdssd|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||false|
|Client Secret|Password||*****|

## Sync Alerts - 12
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||https://api.crowdstrike.com|
|Client ID|String||dssdsdds|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||true|
|Client Secret|Password||*****|

## Sync Alerts - 15
This job will synchronize Google SecOps Alerts and SentinelOne alerts. The job synchronizes status. Requires “SentinelOne Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” you will need to add an “Alert_ID” Alert Context Value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||dssdsddsd|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||true|
|API Token|Password||*****|

## Sync Alerts - 16
This job will synchronize Google SecOps Alerts and SentinelOne alerts. The job synchronizes status. Requires “SentinelOne Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” you will need to add an “Alert_ID” Alert Context Value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||sdssdds|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||false|
|API Token|Password||*****|

## Sync Alerts - 17
This job will synchronize Google SecOps Alerts and SentinelOne alerts. The job synchronizes status. Requires “SentinelOne Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” you will need to add an “Alert_ID” Alert Context Value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||cxcxcx|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||true|
|API Token|Password||*****|

## Sync Alerts - 22d
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||https://api.crowdstrike.com|
|Client ID|String||ssddsdssd|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||true|
|Client Secret|Password||*****|

## Sync Alerts - 3
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||https://api.crowdstrike.com|
|Client ID|String||ssdsssd|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||false|
|Client Secret|Password||*****|

## Sync Alerts - 4
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||https://api.crowdstrike.com|
|Client ID|String||sddssd|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||true|
|Client Secret|Password||*****|

## Sync Alerts - 5
This job will synchronize Google SecOps Alerts and SentinelOne alerts. The job synchronizes status. Requires “SentinelOne Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” you will need to add an “Alert_ID” Alert Context Value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||ssdssd|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||true|
|API Token|Password||*****|

## Sync Alerts - 6
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||https://api.crowdstrike.com|
|Client ID|String||sdssddsds|
|Max Hours Backwards|Int||24|
|Client Secret|Password||*****|
|Verify SSL|Boolean||false|

## Sync Alerts - 8
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||https://api.crowdstrike.com|
|Client ID|String||qwewwewwe|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||false|
|Client Secret|Password||*****|

## Sync Alerts - 9
This job will synchronize Google SecOps Alerts and SentinelOne alerts. The job synchronizes status. Requires “SentinelOne Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” you will need to add an “Alert_ID” Alert Context Value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||sdsddssdsd|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||false|
|API Token|Password||*****|

## Sync Alerts
This job will synchronize Google SecOps Alerts and Crowdstrike alerts. The job synchronizes comments and status. Requires “Crowdstrike Alert” tag on the case. Note: If the alert didn’t originate from “Alerts Connector” or “Identity Protections Detection Connector” you will need to add an “Alert_ID” context value for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||https://api.crowdstrike.com|
|Client ID|String||ssdsdasd|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||true|
|Client Secret|Password||*****|

## Sync Closed Incidents - jaya
This job will synchronize closed ServiceNow incidents and Google SecOps alerts. This job works with ServiceNow incidents that were ingested as alerts and also cases, which contains tag “ServiceNow” and “TICKET_ID” context value with Incident Number inside of it.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Api Root|String||https://{dev-instance}.service-now.com/api/now/v1/|
|Username|String||jhjhjhjjkkjkjjk|
|Verify SSL|Boolean||true|
|Client ID|String||jhhjjh|
|Use Oauth Authentication|Boolean||false|
|Max Hours Backwards|Int||24|
|Table Name|String||jkjkkjkj|
|Password|Password||*****|
|Client Secret|Password||*****|
|Refresh Token|Password||*****|

## Sync Closure
Close tickets in Jira if corresponding Google SecOps alerts were closed.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String||https://{jira_address}|
|Username|String||sdsdds|
|Environment|String|||
|Project Names|String||project names separated by comma|
|Days Backwards|String||1|
|API Token|Password||*****|

## Sync Comments - 19
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String||http://x.x.x.x:<port>|
|Username|String||sdssddssd|
|Summery Field|String||summery.combo_name|
|Ticket Fields|String||summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String||Test|
|Ticket Type Field|Boolean||true|
|Analyst Type Field|Boolean||true|
|Time Stamp Field|Boolean||true|
|Timezone String|Boolean||true|
|Password|Password||*****|

## Sync Comments - 2
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String||http://x.x.x.x:<port>|
|Username|String||tyyuu|
|Summery Field|String||summery.combo_name|
|Ticket Fields|String||summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String||Test|
|Ticket Type Field|Boolean||true|
|Analyst Type Field|Boolean||true|
|Time Stamp Field|Boolean||true|
|Timezone String|Boolean||true|
|Password|Password||*****|

## Sync Comments - 3
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Analyst Type Field|Boolean||true|
|Time Stamp Field|Boolean||true|
|Timezone String|Boolean||true|
|API Root|String||http://x.x.x.x:<port>|
|Username|String||dsdsds|
|Summery Field|String||summery.combo_name|
|Ticket Fields|String||summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String||Test|
|Ticket Type Field|Boolean||true|
|Password|Password||*****|

## Sync Comments - 4
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String||http://x.x.x.x:<port>|
|Username|String||dsdsds|
|Summery Field|String||summery.combo_name|
|Ticket Fields|String||summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String||Test|
|Ticket Type Field|Boolean||true|
|Analyst Type Field|Boolean||true|
|Time Stamp Field|Boolean||true|
|Timezone String|Boolean||true|
|Password|Password||*****|

## Sync Comments - 5
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String||http://x.x.x.x:<port>|
|Username|String||ssdsddssd|
|Summery Field|String||summery.combo_name|
|Ticket Fields|String||summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String||Test|
|Ticket Type Field|Boolean||true|
|Analyst Type Field|Boolean||true|
|Time Stamp Field|Boolean||true|
|Timezone String|Boolean||true|
|Password|Password||*****|

## Sync Comments - 6
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String||http://x.x.x.x:<port>|
|Username|String||hghjjkhjh|
|Summery Field|String||summery.combo_name|
|Ticket Fields|String||summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String||Test|
|Ticket Type Field|Boolean||true|
|Analyst Type Field|Boolean||true|
|Time Stamp Field|Boolean||true|
|Timezone String|Boolean||true|
|Password|Password||*****|

## Sync Comments - 7
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String||http://x.x.x.x:<port>|
|Username|String||ddsdssdsd|
|Summery Field|String||summery.combo_name|
|Ticket Fields|String||summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String||Test|
|Ticket Type Field|Boolean||true|
|Analyst Type Field|Boolean||true|
|Time Stamp Field|Boolean||true|
|Timezone String|Boolean||true|
|Password|Password||*****|

## Sync Comments - 8
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String||http://x.x.x.x:<port>|
|Username|String||dedfdffddf|
|Summery Field|String||summery.combo_name|
|Ticket Fields|String||summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String||Test|
|Ticket Type Field|Boolean||true|
|Analyst Type Field|Boolean||true|
|Time Stamp Field|Boolean||true|
|Timezone String|Boolean||true|
|Password|Password||*****|

## Sync Comments
Sync comments from CA Desk Manager to Siemplify.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String||http://x.x.x.x:<port>|
|Username|String||jj,skskjkj|
|Summery Field|String||summery.combo_name|
|Ticket Fields|String||summery.combo_name,customer.combo_name,category.sym,status.sym,priority.sym,active,log_agent.combo_name,assignee.combo_name,group.combo_name,affected_service.name,severity.sym,urgency.sym,impact.sym,problem.ref_num,resolution_code.sym,call_back_date,change.chg_ref_num,caused_by_chg.chg_ref_num,external_system_ticket,resolution_method.sym,symptom_code.sym,requested_by.combo_name,persistent_id,summary,description,open_date,last_mod_dt,resolve_date,close_date,ref_num|
|Script Name|String||Test|
|Ticket Type Field|Boolean||true|
|Analyst Type Field|Boolean||true|
|Time Stamp Field|Boolean||true|
|Timezone String|Boolean||true|
|Password|Password||*****|

## Sync Incidents - 11
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|Api Root|String|||
|Api Key ID|String||sdssdsdsdsd|
|Max Hours Backwards|Int||24|
|User Mapping JSON|String||{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean||true|
|Api Key|Password||*****|

## Sync Incidents - 111
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|Api Root|String|||
|Api Key ID|String||kjjkkjkj|
|Max Hours Backwards|Int||24|
|User Mapping JSON|String||{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean||true|
|Api Key|Password||*****|

## Sync Incidents - 1s
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|Api Root|String|||
|Api Key ID|String||ss|
|Max Hours Backwards|Int||24|
|User Mapping JSON|String||{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean||true|
|Api Key|Password||*****|

## Sync Incidents - 2
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|Api Root|String||dssdsdsdsd|
|Api Key ID|String||dsdssdsd|
|Max Hours Backwards|Int||24|
|User Mapping JSON|String||{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean||false|
|Api Key|Password||*****|

## Sync Incidents - 22
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|Api Root|String||cxcxcxc|
|Api Key ID|String||sds|
|Max Hours Backwards|Int||24|
|User Mapping JSON|String||{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean||true|
|Api Key|Password||*****|

## Sync Incidents - 3
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|Api Root|String|||
|Api Key ID|String||dssdsdsd|
|Max Hours Backwards|Int||24|
|User Mapping JSON|String||{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean||true|
|Api Key|Password||*****|

## Sync Incidents - 7
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|Api Root|String||ssddsddsds|
|Api Key ID|String||dssdsd|
|Max Hours Backwards|Int||24|
|User Mapping JSON|String||{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean||false|
|Api Key|Password||*****|

## Sync Incidents V2 - 20
Use the Sync Incidents V2 job to synchronize Google SecOps alerts with Microsoft Sentinel incidents. This job ensures that comments, statuses, and tags are synchronized bi-directionally between both systems. Note: Assignee and severity synchronization occurs exclusively from Microsoft Sentinel to Google SecOps. For the job to identify the correct information, the Google SecOps case must have the Microsoft Sentinel Incident tag. This job only works on alerts from the Microsoft Azure Sentinel Incident Connector v2.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|Azure Subscription ID|String||sddssd|
|Azure Active Directory ID|String||dssdsdsds|
|OAUTH2 Login Endpoint Url|String||https://login.microsoftonline.com|
|Management API Root|String||https://msdanagement.azure.com|
|Azure Resource Group|String||sdsdsds|
|Azure Sentinel Workspace Name|String||dssd|
|Client ID|String||dsdsdsdsdds|
|Max Hours Backwards|Int||24|
|Sync Assignee|Boolean||false|
|Verify SSL|Boolean||true|
|Client Secret|Password||*****|

## Sync Incidents
This job synchronizes Google SecOps Alerts and Palo Alto XDR Incidents. It ensures that comments and status are kept in sync between the two systems. For the job to identify the correct information, the Google SecOps case must have the "Palo Alto XDR Incident" tag. If the alert didn’t originate from "Palo Alto Cortex XDR Connector",  you will need to add an "Incident_ID" context value to the case for the job to be able to find the correct information.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|Api Root|String|||
|Api Key ID|String||54|
|Max Hours Backwards|Int||24|
|User Mapping JSON|String||{"Google SecOps Display Name": "XDR Username"}|
|Verify SSL|Boolean||false|
|Api Key|Password||*****|

## Sync Threats - 18
This job will synchronize Google SecOps Alerts and SentinelOne threats. The job synchronizes comments and status. Requires “SentinelOne Threat” tag on the case. Note: If the alert didn’t originate from “Threats Connector” you will need to add an “Threat_ID” Alert Context Value for the job to be able to find the correct information. 


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||dsdsd|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||true|
|API Token|Password||*****|

## Sync Threats - 5
This job will synchronize Google SecOps Alerts and SentinelOne threats. The job synchronizes comments and status. Requires “SentinelOne Threat” tag on the case. Note: If the alert didn’t originate from “Threats Connector” you will need to add an “Threat_ID” Alert Context Value for the job to be able to find the correct information. 


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||fddfdfdf|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||false|
|API Token|Password||*****|

## Sync Threats - 8
This job will synchronize Google SecOps Alerts and SentinelOne threats. The job synchronizes comments and status. Requires “SentinelOne Threat” tag on the case. Note: If the alert didn’t originate from “Threats Connector” you will need to add an “Threat_ID” Alert Context Value for the job to be able to find the correct information. 


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||dssddfdf|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||false|
|API Token|Password||*****|

## Sync Threats
This job will synchronize Google SecOps Alerts and SentinelOne threats. The job synchronizes comments and status. Requires “SentinelOne Threat” tag on the case. Note: If the alert didn’t originate from “Threats Connector” you will need to add an “Threat_ID” Alert Context Value for the job to be able to find the correct information. 


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Environment Name|String||Default Environment|
|API Root|String||ssssdsd|
|Max Hours Backwards|Int||24|
|Verify SSL|Boolean||false|
|API Token|Password||*****|

## Token Renewal Job - 2
Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Integration Environments|String||hello|
|Connector Names|String||hello|

## Token Renewal Job - 4
Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Integration Environments|String||dssddssdds|
|Connector Names|String||sddssd|

## Token Renewal Job
Token renewal job should be used to periodically update the refresh token configured for the integration. By default, the refresh token expires every 90 days, making integration unusable upon expiration. It is recommended to run this job every 7 or 14 days to make sure that refresh token will be up to date.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|Integration Environments|String||jkhhjkhjk|
|Connector Names|String|||

## jira new Sync Closure
Close tickets in Jira if corresponding Google SecOps alerts were closed.


**Run Interval In Seconds:** None

#### Parameters
|Name|Type|Is Mandatory|Value|
|----|----|------------|-----|
|API Root|String||https://{jira_address}|
|Username|String|||
|Environment|String|||
|Project Names|String||project names separated by comma|
|Days Backwards|String||1|
|API Token|Password||*****|

