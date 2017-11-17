# Generalidades de Linux

## Nombres y extensiones de Archivos

* En Linux no existe el concepto de nombre y extensión a la hora de nombrar archivos. 

* El punto es un carácter más permitido en el nombre de un archivo.

##  Las mayúsculas se diferencias de las minúsculas

* Linux es sensible a los casos de las mayúsculas y minúsculas. 

Ejemplo:  myfile, Myfile y myFILE  son tres archivos diferentes.

*  Se aplica esta regla también para la configuración usuario/ contraseña.

## Tipos de Archivos

Ficheros (Archivos)

**Planos** /etc/sysconfig/network (contiene información de configuración)

**Binarios** /bin/ls (contiene información como funciones comunes y gráficos)
 
**Enlaces** /etc/system-release -> /etc/fedora-release (archivos asociados 
 a otros archivos que podría representar la misma data o podrían apuntar 
 a otro archivo, lo que es conocido como enlace directo o shortcut)
(Enlaces "duros",  asocia el nombre del enlace con la información del archivo fuente. 
 Enlace suave es una referencia al nombre de un archivo, no a la información)

**Especiales** /dev/sda1 (representa los diferentes dispositivos del sistema, 
 como discos duros, puertos seriales y particiones montadas en la raíz)



Ficheros (Archivos) -------------------- @ Planos /etc/sysconfig/network @ Binarios /bin/ls @ Enlaces /etc/system-release -> /etc/fedora-release @ Especiales /dev/sda1-->partición montada en la raiz / tty1 . ] . ]--->consolas de texto . ] tty6 ] tty7 --->consola de gráfica tty1 --> Entrar con Ctrl+Alt+F1, para tty3 (Ctrl+Alt+F3) Prompt del Sistema ------------------------------ [alumno@localhost ~] | | |__________________________________________ Ruta del Directorio actual | |_________________________Nombre del Equipo (Hostname) |̣___̣_______ Nombre del usuario 
