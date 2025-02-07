# sqlmap
#plateform/linux #target/remote #cat/ATTACK

## Test GET request
```
sqlmap -u <url> --batch
```

## Test POST request with cookie
```
sqlmap -u <url> --cookie '<cookie>' --data '<data>' --batch
```

## Test request from burp
```
sqlmap -r <req_file> --batch
```
