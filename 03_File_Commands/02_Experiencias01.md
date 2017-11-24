## Primera Experiencia ##

`$> cat /etc/passwd` 

Muestra el contenido de un archivo sin pausa 

`$> tac /etc/passwd` 

Muestra el contenido de un archivo sin pausa pero al reves, lo mismo que cat pero al reves 

`$> more /etc/services` 

Muestra un archivo con pausa por pagina, enter para seguir avanzando 

`$> less /etc/services` 

Muestra un archivo en modo interactivo

`$> tail /etc/passwd` 

Muestra las últimas 10 lineas de un archivo 

`$> tail -1 /etc/passwd` 

Muestra la ultima linea de un archivo 

`$> tail -5 /etc/passwd`

Muestra las ultimas 5 lineas de un archivo 

`$> tail -f /var/log/messages` 

Muestra en forma interactiva los cambios en las ultimas lineas de un archivo: ctrl+c para salir 

`$> cat /etc/services | less` 

Visualiza el contenido del archivo /etc/services y el resultado se concatena en less 

`$> less /etc/services` 

Tiene el mismo resultado que el comando anterior 

`$> cat -n /etc/services | less` 

Lo mismo que los archivos anteriores pero mostrando los numeros de linea 

`$> cat /etc/hosts /etc/redhat-release` 

Concatena la visualizacion de los dos archivos en una sola salida por el stdout (pantalla) 

`$> cat>archivo hola mundo linux es chevere`
 
`ctrl+c` 
usado de esta forma cat actúa como un editor de texto $> cat archivo 

Muestra lo que se escribio anteriormente 

`$> cat /etc/passwd > passwords`

Creando archivo a partir de la salida estandar 

`$> cat /etc/group >> passwords` 

Añade al final del archivo 

`$> grep imap /etc/services ; echo hola` 

Filtra por palabra la visualizacion del archivo ";" se usa para ejecutar otro comando en la misma linea 

`$> wc /etc/services` 

Cuenta el numero de lineas palabras y caracteres del archivo 

`$> wc -l /etc/services` 

Cuenta solo números de lineas 

`$> tail /etc/services` 

Visualiza las 10 ultimas lineas 

`$> tac /etc/services` 

Visualiza de abajo hacia arriba el contenido del archivo 

`$> head /etc/services` 

Visualiza las 10 primeras lineas 

`$> head -8 /etc/services` 

Visualiza las 8 primeras lineas 

`$> tail -1 /etc/passwd` 

Muestra el ultimo usuario creado 

`$> head -30 /etc/services | tail -5` 

Muestra las lineas de la 25 a la 30 

`$> cat /etc/group | tee -a passwords` 

Añade al final del archivo y muestra la salida estandar 

`$> cat /etc/passwd |cut -d ":" -f1` 

Corta las lineas por columna separandolas por ":" y muestra la primera columna 

`$> sed -e "s/smtp/correo/g" /etc/services` 

Reemplaza la palabra smtp por correo (solo en la salida estándar) 

`$> sed -e "s/telnet/conexion remota/g" \ 
-e "s;smtp;correo;g" /etc/services`

Reemplaza la palabra telnet y smpt por correxion remota y correo 

`$> sed -i "s;smtp;correo;g" /etc/services` 

NO EJECUTAR Reemplaza la palabra smtp por correo (modifica el archivo) 

`$> cat /etc/services | tr a-z A-Z` 

Transforma las letras minúsculas a mayúsculas 

`$> cat /etc/passwd | tr -d "[0-9]"` 

Borra los numeros 

`$> cat /etc/passwd | tr -c "[a-z A-Z]" "-"` 

Transforma los caracteres que no sean letras en "-" 

`$> cat /etc/services |tr -s "\n*"` 

Transforma los saltos de lineas consecutivas en uno solo (elimina linea en blanco) 

`$> pr /etc/services` 

Visualiza en formato de impresión 

`$> pr /etc/services | less` 

`$> pr /etc/services > /dev/lp0` 

Impresión del archivo /etc/services 

`lp0 es el puerto paralelo` 

## Búsqueda de Archivos ##
### find,locate,whereis ###

`$> find ./ -name a\* `

Busca archivos y directorios que comiencen con a, tomando como base el directorio actual 

`$> find /etc -name hosts` 

Busca desde el /etc el archivo o directorio interfaces 

`$> find /usr -name "*" -size +300k` 

Busca todos los archivos en el /usr que pesen mas de 300K 

`$> find /etc -name passwd -exec cat {} \;` 

Busca todo los archivos llamados passwd dentro de /etc y luego visualiza el contenido de cada uno de ellos con el comando cat 

`$> find / -user alumno -size 3M` 

Busca archivos del usuario alumno que sean mayores a 3 Megas en todo el sistema 

`$> updatedb` 

Actualiza la base de datos de la lista de archivos y directorios existentes en el sistema 

`$> locate interfaces` 

Busca en la base de datos el archivo interfaces 

`$> whereis vi` 

Muestra la ruta de binarios, librerias y documentacion del comando vi 

`$> which vi` 

Muestra la ruta del binario del comando vi
