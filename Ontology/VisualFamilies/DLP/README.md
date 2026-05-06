<p align="center">
<img src="./DLP.png" 
     alt="DLP" width="200"/></p>
     
# DLP

### Description
Unauthorized data exfiltration

### Rules
|Primary Source|Secondary Source|Third Source|Forth Source|Type|Primary Destination|Secondary Destination|Third Destination|Forth Destination|
|--------------|----------------|------------|------------|----|-------------------|---------------------|-----------------|-----------------|
|USB|DestinationHostName|DestinationAddress||Type|DestinationHostName|DestinationAddress|USB||
|DestinationHostName|DestinationAddress|||Linked|DestinationUserName||||
|DestinationHostName||||Linked|DestinationAddress||||
