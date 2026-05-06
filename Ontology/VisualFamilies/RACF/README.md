<p align="center">
<img src="./RACF.png" 
     alt="RACF" width="200"/></p>
     
# RACF

### Description
Mainframe resource access

### Rules
|Primary Source|Secondary Source|Third Source|Forth Source|Type|Primary Destination|Secondary Destination|Third Destination|Forth Destination|
|--------------|----------------|------------|------------|----|-------------------|---------------------|-----------------|-----------------|
|SourceUserName|DestinationProcessName|||Type|DestinationProcessName|FileName|SourceUserName||
|SourceUserName||||Linked|SourceProcessName||||
|DestinationProcessName||||Linked|FileName||||
