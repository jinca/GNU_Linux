# Introducción a Software Libre y GNU/Linux 

## Richard Stallman [RMS](https://en.wikipedia.org/wiki/Richard_Stallman#/media/File:NicoBZH_-_Richard_Stallman_(by-sa)_(10).jpg) 
================

Richard Stallman creó el movimiento del Software Libre con el proyecto [GNU](https://www.gnu.org/) (GNU not UNIX) que intentaba crear un sistema operativo superior a Unix y que fuera completamente Libre.
Por ello creó el proyecto GNU en 1983 y la Fundación de Software Libre [(FSF](http://www.fsf.org/ )) en 1985, donde estableció de un marco de referencia moral,político y legal para el movimiento del software libre, como una alternativa al desarrollo y distribución del software no libre o privativo.

:arrow_right: Fruto de este trabajo se creó la licencia GPL y LPGL. 

La GPL establece 4 libertades: 

* Libertad 0: la libertad de usar el programa, con cualquier propósito. 
* Libertad 1: la libertad de estudiar cómo funciona el programa y modificarlo, adaptándolo a tus necesidades. 
* Libertad 2: la libertad de distribuir copias del programa, con lo cual puedes ayudar a tu prójimo. 
* Libertad 3: la libertad de mejorar el programa y hacer públicas esas mejoras a los demás, de modo que toda la comunidad se beneficie.

Cuando uno publica o distribuye un software bajo la GPL esta obligado a publicar el código fuente del mismo. Quien recibe el software puede modificarlo a su gusto; pero no puede redistribuir el código modificado sin que estas tengan el código fuente de sus modificaciones, con lo cual se asegura la libertad del usuario. 
Sin embargo lo que no obliga la GPL, es que tu tengas que publicar obligatoriamente las modificaciones del software GPL que hayas tomado como base. 
Por ejemplo Google gana miles de millones de dólares usando Linux y software libre (GPL y otros) pero solo publica un porcentaje muy limitado de sus proyectos internos. 

Licencias:
https://www.gnu.org/licenses/

Linus Torlvalds
===============

Figura:
https://en.wikipedia.org/wiki/Linus_Torvalds#/media/File:Linus_Torvalds.jpeg

- En 1991, en Helsinki, Linus Torvalds comenzó un proyecto que más tarde se llegó a ser el núcleo Linux; en ese instante el no sabía la dimensión que iba a alcanzar su proyecto. 

- A fines de 1992, Linux libera su kernel con la licencia GPL, consiguiendo que el Sistema Operativo lograra un crecimiento espectacular.

- Linux como proyecto es solamente el núcleo (kernel) del sistema operativo; la combinación con las herramientas de GNU (compilador de C, bash, el debugger) ha creado la base para desarrollar las distribuciones; por eso es común referirse a Linux como GNU/Linux. 

- Las distribuciones toman en un momento determinado una versión del kernel de Linux y la combinan con herramientas GNU, le crean un instalador y herramientas de administración, algunas distribuciones se basan en otras distribuciones y le dan un valor añadido. 

Video OS Revolution:
https://www.youtube.com/watch?v=sujZg7jwKdk


Distribuciones
==============

Sin embargo del universo de distribuciones las más importantes; por su relevancia e influencia en las demás distribuciones, son dos: 
Debian (basado en deb y apt) y Red Hat (basado en rpm y yum). 

Mapa de Distribuciones 
----------------------

* Distribuciones Debian (Servidor) |Red Hat 

Ubuntu (Distro mas popular) | Fedora (Escritorio) 
   Desktop (Escritorio) | RHEL (Servidor) 

      Server (Servidor) | CentOS (clon de RHEL) 
                        | Oracle Linux (Clon de RHEL) 
                        | Scientific Linux (Clon de RHEL) 
 Linux Mint(Escritorio) |SuSE 
       Basado en Ubuntu | OpenSuSE (Escritorio) 
                        | SLES (Servidor) 
                        |Mageia (Escritorio) 

Otros: Slackware, Gentoo, DanSmall Linux, etc 

- Debian representa el éxito de la comunidad, garantizando la libertad de sus usuarios y apoyo desinteresado de los mismos para hacer de Debian una distribución de excelente calidad. 

- Red Hat representa el éxito de la empresa y consolida a Linux dentro de los servidores corporativos. 

Linux: ------> Tiene su propio sistema de archivos ext2,ext3,ext4,btrfs 

Swap --> es una memoria virtual en el disco duro Linux soporta: FAT, NTFS, JFS, XFS Para instalar en linux se necesita como mínimo una particion Swap y una partición raíz. 

Directorios: 
===========

/ ----> raiz 
/boot ----> directorio de arranque del sistema operativo configuración de grub 
/etc  ----> archivos de configuración 
/home ----> directorios de los usuarios 
/usr ----> binarios,librerías,documentacion 
/var ----> archivos que crecen o modifican (correo,base de datos, logs) 
/dev ----> referencia de los perifericos (hardware) 
/proc ----> directorio temporal con punteros a los recursos fisicos de la computadora 
/root ----> directorio principal de Dios 
/tmp ----> directorio temporal 
/opt ----> algunos programas instalan aquí 
/mnt --|>[sirven para mostrar dispositivos de media, unidades de red. 
/media--|

???  Indicar que hay en la carpeta /bin y /dev 

Importancia de GNU/Linux
========================

Todas las supercomputadoras del TOP500 liderada por China, utilizan Linux:
https://fossbytes.com/top-500-linux-supercomputers-list-2017/

Android ha nacido basado en el kernel de Linux
https://en.wikipedia.org/wiki/Android_(operating_system)

Ha dado lugar a la creación de Hardware Libre como Arduino, bajo la licencia LGPL
https://www.arduino.cc/en/Main/FAQ#toc2

Desde hace más de 20 años, muchas comunidades de software libre han nacido para dar soporte a las diferentes distribuciones
http://www.linux-magazine.com/Online/Blogs/Off-the-Beat-Bruce-Byfield-s-Blog/What-makes-for-a-community-distribution

Linux es educación
https://opensource.com/education/14/9/linux-education-public-school

Ahorra energía
http://linrunner.de/en/tlp/docs/tlp-linux-advanced-power-management.html

Open Source vs Software Libre
=============================

En 1997, Eric Raymond escribe "La catedral y el Bazar", este ensayo analiza dos modelos de producción de software bien diferenciados. Por un lado, la catedral, que representa el modelo de desarrollo más hermético y vertical característico del Software propietario; y por el otro el bazar, con su dinámica horizontal y "bulliciosa", que caracterizó al desarrollo del kernel Linux y otros proyectos de software libre que se potenciaron con el trabajo comunitario a través de Internet del código abierto.

Es una figura líder en el Movimiento del Open Source y el Código abierto.

Diferencias:
-----------

- El Software Libre hace hincapié en cuestiones éticas y morales relacionadas con el software, viendo el aspecto técnico como secundario, a diferencia del movimiento Open Source que lo establece como prioritario.

- Con una aplicación desarrollada bajo los estándares del Software Libre puedes obtener remuneración por conceptos de desarrollo, soporte y puesta a punto siempre y cuando entregues los fuentes, a diferencia del movimiento Open Source que no te obliga a hacerlo. Todos los productos desarrollados en Software Libre así como sus derivados siempre deben ser libres, a diferencia de Open Source. 

Extraído del [blog](https://hipertextual.com/archivo/2014/05/diferencias-software-libre-y-open-source/)
