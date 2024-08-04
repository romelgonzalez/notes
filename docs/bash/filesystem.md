#### Ver tamaño de un directorio:  
``` bash
du -sh
```

#### Ver espacio ocupado excluyendo un directorio:  
``` bash
du -shx /\* --exclude=/var/www | sort -rh 
```

#### Ver tamaño de todos las carpetas dentro de un directorio: 
``` bash
du -h --exclude=/proc --max-depth=1 /directorio | sort -rh
```

#### Listar por tamaño los archivos dentro de un directorio: 
``` bash
ls -lh | sort -rh -k5
```

#### Eliminar archivos e el directorio que tengan mas de 7 dias: 
``` bash
find . -type f -mtime +7 -exec rm {} \;
```

#### Buscar un directorio especifico: 
``` bash
find / -type d -name "documentos"
```

#### Buscar un archivo especifico: 
``` bash
find / -type f -name "documento.txt"
```

#### Ver el id de usuario y grupo de directorio: 
``` bash
stat -c '%u:%g' /ruta/directorio
```

#### Copiar scp de local a remoto  
``` bash
scp -i ~/.ssh/llave /ruta-local user@ip:/ruta-remota  
```

#### Copiar scp de remoto a local:  
``` bash 
scp -i ~/.ssh/llave user@ip-server:/ruta-remota .
``` 
El punto indica que se copia en la ubicacion actual

