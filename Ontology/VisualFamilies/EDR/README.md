<p align="center">
<img src="./EDR.png" 
     alt="EDR" width="200"/></p>
     
# EDR

### Description
Endpoint events

### Rules
|Primary Source|Secondary Source|Third Source|Forth Source|Type|Primary Destination|Secondary Destination|Third Destination|Forth Destination|
|--------------|----------------|------------|------------|----|-------------------|---------------------|-----------------|-----------------|
|SourceProcessName|FileName|DestinationHostName||Type|DestinationHostName|DestinationAddress|SourceProcessName||
|SourceProcessName|FileName|||Linked|FileName|FileHash|||
|FileName||||Linked|FileHash||||
|DestinationHostName||||Linked|DestinationAddress||||
|DestinationHostName|DestinationAddress|||Linked|DestinationUserName||||
