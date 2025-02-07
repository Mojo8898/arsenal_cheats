# snmpbulkwalk
#plateform/linux #target/remote #cat/ATTACK

## Enumerate public community string
```
snmpbulkwalk -Cr1000 -c public -v2c <ip> . > snmpwalk.out
```

## Enumerate specified community string
```
snmpbulkwalk -Cr1000 -c <com_str> -v2c <ip> . > snmpwalk.out
```
