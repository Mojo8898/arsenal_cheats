# ffuf
#plateform/linux #target/remote #cat/ATTACK

## Fuzz vhosts
```
ffuf -w /usr/share/seclists/Discovery/DNS/subdomains-top1million-5000.txt -u http://<target> -H 'Host: FUZZ.<target>'
```

## Fuzz entrypoint
```
ffuf -w /usr/share/seclists/Discovery/Web-Content/raft-small-words.txt -u http://<target>/FUZZ
```

## Fuzz extensions
```
ffuf -w /usr/share/seclists/Discovery/Web-Content/web-extensions.txt -u http://<target>/indexFUZZ
```
