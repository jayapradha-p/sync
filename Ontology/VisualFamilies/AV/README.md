<p align="center">
<img src="./AV.png" 
     alt="AV" width="200"/></p>
     
# AV

### Description
Anti-virus alerts visualization

### Rules
|Primary Source|Secondary Source|Third Source|Forth Source|Type|Primary Destination|Secondary Destination|Third Destination|Forth Destination|
|--------------|----------------|------------|------------|----|-------------------|---------------------|-----------------|-----------------|
|DestinationHostName|DestinationAddress|||Type|DestinationHostName|DestinationAddress|||
|DestinationHostName||||Linked|DestinationAddress||||
|DestinationHostName|DestinationAddress|||Linked|DestinationUserName||||
|DestinationHostName|DestinationAddress|||Linked|FileName|FileHash|ThreatSignature||
|FileName||||Linked|FileHash||||
|FileName|FileHash|||Linked|ThreatSignature||||
|FileName|FileHash|||Linked|DestinationProcessName||||
