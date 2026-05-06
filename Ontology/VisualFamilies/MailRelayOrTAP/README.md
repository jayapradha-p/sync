<p align="center">
<img src="./MailRelayOrTAP.png" 
     alt="MailRelayOrTAP" width="200"/></p>
     
# MailRelayOrTAP

### Description
Email monitoring event

### Rules
|Primary Source|Secondary Source|Third Source|Forth Source|Type|Primary Destination|Secondary Destination|Third Destination|Forth Destination|
|--------------|----------------|------------|------------|----|-------------------|---------------------|-----------------|-----------------|
|SourceUserName|SourceHostName|SourceAddress||Type|DestinationUserName|DestinationHostName|DestinationAddress||
|SourceUserName||||Linked|SourceHostName|SourceAddress|||
|SourceHostName||||Linked|SourceAddress||||
|DestinationUserName||||Linked|DestinationHostName|DestinationAddress|||
|DestinationHostName||||Linked|DestinationAddress||||
|DestinationUserName|SourceUserName|||Linked|EmailSubject||||
|DestinationUserName|SourceUserName|||Linked|DestinationURL||||
|DestinationUserName|SourceUserName|||Linked|ThreatSignature||||
|DestinationUserName|SourceUserName|||Linked|FileName||||
|FileName||||Linked|FileHash||||
