## Crear usuarios ##

Crea un nuevo usuario, su directorio de trabajo y su grupo igual 
`$> useradd -md /home/tuxito tuxito` 

Crea o cambia la contraseña de un usuario 
`$> passwd tuxito` 

Se loguea como tuxito 
`$> su - tuxito` 

Muestra información del usuario actual 
`$> id` 

Sale de la sesión 
`$> exit` 

$> id 

Crea usario linuxero con descripcion, grupo principal y grupos adicionales, así como su intérprete de comandos 
`$> useradd -md /home/linuxero -c "linuxero fanatico" \ 
-g users -G video,audio -s /bin/bash linuxero` 

Configura el password parael usuario linuxero
`$> passwd linuxero` 

`$> grep linuxero /etc/passwd` 
 > linuxero:x:1003:100:linuxero fanatico:/home/linuxero:/bin/bash

> Donde: linuxero = nombre del usuario 
> x = la clave del usuario esta en /etc/shadow 
> 1003 = uid del usuario 
> 100 = gid del usuario 
> linuxero fanatico = descripción 
> /home/linuxero = directorio de trabajo del usuario 
> /bin/bash = interpretes de comandos 

`$> grep users /etc/group` 
> users:x:100:pepito,tuxito,windozero 

> Donde: users = nombre del grupo 
> x = la clave del grupo esta en /etc/gshadow (no es comun) 
> 100 = gid del grupo 
> pepito,tuxito,windozero = usuarios adicionales del grupo 

`$> grep linuxero /etc/shadow` (archivo de contraseñas) 
> linuxero:$6$qf7G8CbU$R9wiKgiN0rVaP1qsjQnzRsYfywP3L468:15297:0:99999:7::: 

> Donde: linuxero = nombre del usuario 
> $6$qf7G... = contraseña encriptada en un algoritmo como MD5, SSHA 
> 15297:0:99999:7::: = validación expiración de la contraseña 

## Archivos importantes ##

/etc/passwd (lista de usuarios) 

/etc/group (lista de grupos)

/etc/shadow (lista de contraseñas) 

## Modificar usuarios ##

$> grep tuxito /etc/passwd 

$> usermod -c "tuxito hacker" 
tuxito (modificamos a sus usuarios) 

$> grep tuxito /etc/passwd 

$> vim /etc/passwd (modifica el archivo de usuario) 

## Borrar usuarios ##

$> userdel linuxero (borra el usuario pero no su directorio de trabajo) 

$> userdel -r tuxito (borra el usuario incluyendo su directorio)
