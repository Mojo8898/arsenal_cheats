# sqlmap
#plateform/linux #target/remote #cat/ATTACK

## Send an email
```
swaks -t <target_user>@<target_domain> -f <from_user>@<from_domain> -h 'Subject: IMPORTANT' --body '<body>' -s <ip>
```

## Send an email with attachment
```
swaks -t <target_user>@<target_domain> -f <from_user>@<from_domain> --attach @example.txt -h 'Subject: IMPORTANT' --body '<body>' -s <ip>
```

## Include authentication
```
swaks -t <target_user>@<target_domain> -f <from_user>@<from_domain> -au <user>@<domain> -ap '<passwd>' -h 'Subject: IMPORTANT' --body '<body>' -s <ip>
```

## Include domain
```
swaks -t <target_user>@<target_domain> -f <from_user>@<from_domain> -au <user>@<domain> -ap '<passwd>' -h 'Subject: IMPORTANT' --body '<body>' -s <ip> --ehlo <domain>
```
