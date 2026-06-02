
# Zendesk

Zendesk Support is a beautifully simple system for tracking, prioritizing, and solving customer support tickets.

Python Version - V3_11
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Server Address|None|True|String|https://{username}.zendesk.com|
|User Email Address|None|True|String||
|Api Token|None|True|Password|*****|


#### Dependencies
| |
|-|
|TIPCommon-1.0.11-py2.py3-none-any.whl|
|charset_normalizer-3.3.2-py3-none-any.whl|
|idna-3.7-py3-none-any.whl|
|certifi-2024.2.2-py3-none-any.whl|
|requests-2.31.0-py3-none-any.whl|
|six-1.16.0-py2.py3-none-any.whl|
|chardet-5.2.0-py3-none-any.whl|
|urllib3-2.2.1-py3-none-any.whl|


## Actions
#### Create Ticket
Create a ticket with specific properties
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Description|Description|True|String||
|Assigned User|User full name.|False|String||
|Assignment Group|Group name.|False|String||
|Subject|Subject|True|String||
|Priority|Priority will be one of the following: urgent, high, normal or low.|False|String||
|Ticket Type|The ticket type will be one of the following: problem, incident, question or task.|False|String||
|Tag|Tag|False|String||
|Internal Note|Specify whether the comment should be public, or internal. Unchecked means it will be public, checked means it will be internal only.|False|Boolean|False|
|Email CCs|Specify a comma-separated list of email addresses, which should also receive the notification of the ticket creation. Note: at max 48 email CCs can be added. This is Zendesk limitation.|False|String||
|Validate Email CCs|If enabled, action will try to check that users with emails provided in “Email CCs“ parameter exist. If at least one user doesn’t exist, action will fail. If this parameter is disabled, action will not perform this check.|False|Boolean|true|



#### Update Ticket
Update existing ticket details
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Ticket ID|Ticket number.|True|String|None|
|Subject|The subject of the ticket.|False|String|None|
|Assigned User|User full name.|False|String|None|
|Assignment Group|Group name.|False|String|None|
|Priority|Priority will be one of the following: urgent, high, normal or low.|False|String||
|Ticket Type|The ticket type will be one of the following: problem, incident, question or task.|False|String||
|Tag|Tag to add to the ticket.|False|String||
|Status|The status will be one of the following: new, open, pending, hold, solved or closed.|False|String||
|Internal Note|Specify whether the comment should be public, or internal. Unchecked means it will be public, checked means it will be internal only.|False|Boolean|False|
|Additional Comment|If you want to add a comment to the ticket, specify the text you would like to add as a comment here.|False|String||



#### Ping
Test Connectivity
Timeout - 600 Seconds



#### Get Ticket Details
Get ticket details, comments, and attachments by ticket id
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Ticket ID|The ID f the ticket.|True|String|None|



#### Apply Macros On Ticket
Apply macro to a ticket
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Ticket ID|Ticket number.|True|String|None|
|Macro Title|Macro Title|True|String|None|



#### Search Tickets
Search tickets by keyword
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Search Query|Query content(e.g: type:ticket status:pending).|True|String||



#### Add Comment To Ticket
Add a comment to an existing ticket
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Ticket ID|Specify the Zendesk Ticket ID for which you would like to add a comment.|True|String||
|Comment Body|Provide the text you would like to be contained in the comment body|True|Content||
|Author Name|Specify the name of the author, please make sure this name exists on Zendesk|False|String|None|
|Internal Note|Specify whether the comment should be public, or internal. Unchecked means it will be public, checked means it will be internal only.|False|Boolean||









