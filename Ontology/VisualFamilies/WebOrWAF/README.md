<p align="center">
<img src="./WebOrWAF.png" 
     alt="WebOrWAF" width="200"/></p>
     
# WebOrWAF

### Description
Suspicious pageRequest of internal web resource

### Rules
|Primary Source|Secondary Source|Third Source|Forth Source|Type|Primary Destination|Secondary Destination|Third Destination|Forth Destination|
|--------------|----------------|------------|------------|----|-------------------|---------------------|-----------------|-----------------|
|SourceUserName|SourceHostName|SourceAddress||Type|DestinationHostName|DestinationAddress|SourceUserName||
|SourceUserName|SourceHostName|SourceAddress||Linked|ThreatSignature||||
|SourceUserName||||Linked|SourceHostName|SourceAddress|||
|SourceHostName||||Linked|SourceAddress||||
|DestinationHostName||||Linked|DestinationAddress||||
|DestinationHostName|DestinationAddress|||Linked|DestinationURL||||
