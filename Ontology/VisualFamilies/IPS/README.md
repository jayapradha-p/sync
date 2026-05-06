<p align="center">
<img src="./IPS.png" 
     alt="IPS" width="200"/></p>
     
# IPS

### Description
Suspicious traffic events

### Rules
|Primary Source|Secondary Source|Third Source|Forth Source|Type|Primary Destination|Secondary Destination|Third Destination|Forth Destination|
|--------------|----------------|------------|------------|----|-------------------|---------------------|-----------------|-----------------|
|SourceHostName|SourceAddress|DestinationHostName||Type|DestinationHostName|DestinationAddress|SourceHostName||
|SourceHostName||||Linked|SourceAddress||||
|DestinationHostName||||Linked|DestinationAddress||||
|SourceHostName|SourceAddress|||Linked|ThreatSignature||||
