<p align="center">
<img src="./InsiderThreat.png" 
     alt="InsiderThreat" width="200"/></p>
     
# InsiderThreat

### Description
Suspicious internal activity

### Rules
|Primary Source|Secondary Source|Third Source|Forth Source|Type|Primary Destination|Secondary Destination|Third Destination|Forth Destination|
|--------------|----------------|------------|------------|----|-------------------|---------------------|-----------------|-----------------|
|SourceUserName|SourceHostName|SourceAddress||Type|FileName|SourceUserName|SourceHostName||
|SourceUserName||||Linked|SourceHostName|SourceAddress|||
|SourceHostName||||Linked|SourceAddress||||
