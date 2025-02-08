# FFUF 
#plateform/linux #target/remote #cat/enum



## FFUF subdomain checking
#plateform/linux #target/remote #cat/enum
```
ffuf -w /usr/share/seclists/Discovery/DNS/subdomains-top1million-110000.txt -H "Host: FUZZ.<domain>.<ending>" -u https://<domain.here>
```