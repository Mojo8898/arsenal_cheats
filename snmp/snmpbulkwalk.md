# snmpbulkwalk
#plateform/linux #target/remote #cat/ATTACK

## Enumerate public community string
```
snmpbulkwalk -Cr1000 -c <community_string|public> -v2c <ip> . > snmpwalk.out
```
