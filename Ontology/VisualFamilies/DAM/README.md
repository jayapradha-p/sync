<p align="center">
<img src="./DAM.png" 
     alt="DAM" width="200"/></p>
     
# DAM

### Description
Suspicious user activity on a database object

### Rules
|Primary Source|Secondary Source|Third Source|Forth Source|Type|Primary Destination|Secondary Destination|Third Destination|Forth Destination|
|--------------|----------------|------------|------------|----|-------------------|---------------------|-----------------|-----------------|
|SourceUserName|SourceHostName|SourceAddress||Type|DestinationHostName|DestinationAddress|SourceUserName||
|SourceUserName|SourceHostName|SourceAddress||Linked|ThreatSignature||||
|SourceUserName||||Linked|SourceHostName|SourceAddress|||
|SourceHostName||||Linked|SourceAddress||||
|DestinationHostName||||Linked|DestinationAddress||||
|DestinationHostName|DestinationAddress|||Linked|FileName||||
