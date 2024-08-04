#### Crear llaves ssh:  
``` bash
ssh-keygen -f ~/.ssh/nombre -t rsa -b 4096 -C nombre 
ssh-keygen –t ed25519 –a 200 -C [nombre] -f ~/.ssh/[nombre] (nueva version recomendada)
```

#### Convertir llave publica .pub a .pem: 
``` bash
ssh-keygen -f user_id_rsa.pub -e -m PEM > pubkey.pem
```

#### Convertir certificado a .pfx  
``` bash
openssl pkcs12 -export -out certificado.pfx -inkey private.key -in certificado.crt
```

#### Conexion ssh error de demasiadas autenticaciones fallidas:  
``` bash
ssh -o IdentitiesOnly=yes servidor@ip
ssh-keygen -R ip (renovar llave temporal para conexion)
```


#### Sacar hash del Key: 
``` bash
openssl pkey -in llave.key -pubout -outform pem | sha256sum
```

#### Sacar hash de la crt:  
``` bash
openssl x509 -in certificado-antiguo.crt -pubkey -noout -outform pem | sha256sum
```

#### Sacar hash del csr: 
``` bash
openssl req -in CSR.csr -pubkey -noout -outform pem | sha256sum
```

#### Genrerar CSR:  
``` bash
openssl req -out banda-l.csr -new -newkey rsa:4096 -keyout private.key
```




``` bash

```