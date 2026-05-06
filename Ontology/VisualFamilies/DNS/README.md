<p align="center">
<img src="./DNS.png" 
     alt="DNS" width="200"/></p>
     
# DNS

### Description
Review Active Directory DNS events

### Rules
|Primary Source|Secondary Source|Third Source|Forth Source|Type|Primary Destination|Secondary Destination|Third Destination|Forth Destination|
|--------------|----------------|------------|------------|----|-------------------|---------------------|-----------------|-----------------|
|SourceHostName|SourceAddress|DestinationHostName||Type|DestinationHostName|DestinationAddress|SourceHostName||
|SourceHostName||||Linked|SourceAddress||||
|DestinationHostName||||Linked|DestinationAddress||||
