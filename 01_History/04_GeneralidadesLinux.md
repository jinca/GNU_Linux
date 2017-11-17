# Generalidades de Linux

## Nombres y extensiones de Archivos

* En Linux no existe el concepto de nombre y extensión a la hora de nombrar archivos. 

* El punto es un carácter más permitido en el nombre de un archivo.

##  Las mayúsculas se diferencias de las minúsculas

* Linux es sensible a los casos de las mayúsculas y minúsculas. 

Ejemplo:  myfile, Myfile y myFILE  son tres archivos diferentes.

*  Se aplica esta regla también para la configuración usuario/ contraseña.

## Tipos de Archivos

**Planos** /etc/sysconfig/network (contiene información de configuración)

**Binarios** /bin/ls (contiene información como funciones comunes y gráficos)
 
**Enlaces** /etc/system-release -> /etc/fedora-release (archivos asociados 
 a otros archivos que podría representar la misma data o podrían apuntar 
 a otro archivo, lo que es conocido como enlace directo o shortcut)
(Enlaces "duros",  asocia el nombre del enlace con la información del archivo fuente. 
 Enlace suave es una referencia al nombre de un archivo, no a la información)

**Especiales** /dev/sda1 (representa los diferentes dispositivos del sistema, 
 como discos duros, puertos seriales y particiones montadas en la raíz)

## Files everywhere!!!

¿Qué pasa con los directorios o folders?

Los directorios son archivos especiales que sirven como almacenador para organizar otros archivos.

Cuando se crea un directorio, un file o archivo es colocado en el disco duro para representar dicho directorio.

## Consolas de texto y gráfica

tty1 (Presionando Ctrl+Alt+F1)  ---> consola de texto

tty2 (Presionando Ctrl+Alt+F2)  ---> consola de texto

tty3 (Presionando Ctrl+Alt+F3)  ---> consola de texto

tty4 (Presionando Ctrl+Alt+F4)  ---> consola de texto

tty5 (Presionando Ctrl+Alt+F5)  ---> consola de texto

tty6 (Presionando Ctrl+Alt+F6)  ---> consola de texto

tty7 (Presionando Ctrl+Alt+F7)  ---> consola gráfica


## Prompt del Sistema 

<p align="center">
<img src="https://github.com/jinca/GNU_Linux/blob/master/Images/prompt.png">
</p>

## Rutas de Directorios

**Ruta Absoluta**

Aquella ruta que se toma en cuenta desde la raíz 

Ejemplo: 

$> ls /etc/fedora-release 


**Ruta Relativa**

Aquella ruta que se toma en cuenta desde el directorio actual 


_Responder:_

`$> cd /etc`
 
`$> ls fedora-release` 

`$> ls ../usr/share/doc` 

`$> ls .`

`$> cat /etc/passwd`

<p align="center">
<img src="https://github.com/jinca/GNU_Linux/blob/master/Images/passwd.png">
</p>


## Autocompletar

* Autocompleta Rutas (Absolutas y Relativas de archivos de archivos) 

* Autocompleta nombres de comandos. Ejemplo: `ca <TAB>` 

* Autocompleta nombres de variables de entorno. Ejemplo: `HOST <TAB>`
