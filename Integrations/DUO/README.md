
# DUO

Cisco's MFA Solution. Duo is engineered to provide a simple, streamlined login experience for every user and application, and as a cloud-based solution, it integrates easily with your existing technology.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Hostname|API hostname for your tenant: api-XXXXXXXX.duosecurity.com.|True|String|api-XXXXXXXX.duosecurity.com|
|Admin Secret Key|The Duo Admin API provides programmatic access to the administrative functionality of Duo Security's two-factor authentication platform.https://duo.com/docs/adminapi|True|Password|*****|
|Admin Integration Key|The Duo Admin API provides programmatic access to the administrative functionality of Duo Security's two-factor authentication platform.https://duo.com/docs/adminapi|True|Password|*****|
|Auth Integration Key|The Duo Auth API is a low-level, RESTful API for adding strong two-factor authentication to your website or application.https://duo.com/docs/authapi|True|Password|*****|
|Auth Secret Key|The Duo Auth API is a low-level, RESTful API for adding strong two-factor authentication to your website or application.https://duo.com/docs/authapi|True|Password|*****|


#### Dependencies
| |
|-|
|duo_client-5.3.0-py3-none-any.whl|
|six-1.17.0-py2.py3-none-any.whl|
|setuptools-80.9.0-py3-none-any.whl|


## Actions
#### Get Trust Monitor Events
Returns DUO Trust Monitor events from the last X days
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Number Days Back|Number of days back to pull events from|True|String|1|



#### Ping
Uses the /check endpoint to verify that the Auth API integration and secret keys are valid, and that the signature is being generated properly.
Timeout - 600 Seconds



#### Get Authentication Logs for User
Obtains the user data and authentication logs for a specified user over a number of days from now.
Also outputs lists of authentication sources that match a threshold (default 2). Useful to help determine if an auth source is normally seen.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Authentication Threshold|Number of successful authentications to indicate a source may be from a known safe entity.|True|String|2|
|Number Days Back|Number of days back to obtain authentication logs from.Default 1 day|True|String|1|
|Username|Username to retrieve logs for.|False|String||



#### Get Users by Name
Query the get_users_by_name DUO API endpoint to obtain information on a specified username.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Username|Username|True|String|admin|









## Connectors
#### DUO - Trust Monitor Connector
Creates cases from last X days of DUO Trust Monitor Events.
https://duo.com/docs/adminapi#trust-monitor

|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Days Back|The max days back to retrieve data from|True|Int|1|
|API Hostname|API hostname for your tenant: api-XXXXXXXX.duosecurity.com.|True|String|api-XXXXXXXX.duosecurity.com|
|Admin Secret Key|DUO Admin API Secret Keyhttps://duo.com/docs/adminapi|True|Password|*****|
|Admin Integration Key|DUO Admin API Integration Keyhttps://duo.com/docs/adminapi|True|Password|*****|




