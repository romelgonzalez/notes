

#### Ver puertos abiertos:  
``` bash
netstat -plnut
```

#### Ver conexiones:
``` bash
ss -tunap
netstat -nputw
```

#### Verificar un puerto:  
``` bash
ss -pnltue | grep 8000
```

#### Ver quien resuleve DNS: 
``` bash
dig +short myip.opendns.com @resolver1.opendns.com
```


``` bash

```
