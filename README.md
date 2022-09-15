# Docker

vamos a documentar todas las actividades realizadas
en el laboratorio.
# Aquitectura

La virtualización basada en contenedores, también llamada virtualización del sistema operativo, 
es una aproximación a la virtualización en la cual la capa de virtualización se ejecuta como una aplicación en el sistema operativo (OS).

 Diagrama De Bloques

![arquitectura bloques](https://user-images.githubusercontent.com/100426946/187724083-226fd1de-0ab0-4328-a485-ae401a14e673.jpg)

# workflow
El ciclo de vida de desarrollo de una aplicación se inicia en el equipo de cada desarrollador, donde se programa la aplicación con el lenguaje preferido y se prueba en el entorno local. Con este flujo de trabajo, no importa el lenguaje, el marco ni la plataforma que se elija, ya que siempre se desarrollan y se prueban contenedores de Docker en local.

Cada contenedor (una instancia de una imagen de Docker) incluye los siguientes componentes:

Una selección de sistema operativo, por ejemplo, una distribución de Linux, Windows Nano Server o Windows Server Core.

Archivos agregados durante el desarrollo, por ejemplo, archivos binarios de código fuente y aplicación.

Información de configuración, como configuración de entorno y dependencias.



En esta sección se explica el flujo de trabajo de desarrollo de bucle interno para aplicaciones basadas en contenedor de Docker. Flujo de trabajo de bucle interno significa que no se tiene en cuenta el flujo de trabajo general de DevOps, que puede incluir hasta implementación en producción, y solo se centra en el trabajo de desarrollo realizado en el equipo del desarrollador. Los pasos iniciales para configurar el entorno no se incluyen, ya que se realizan solo una vez.

Una aplicación se compone de sus propios servicios, además de bibliotecas adicionales (dependencias). Estos son los pasos básicos que normalmente se realizan al compilar una aplicación de Docker,
 
![flujo](https://user-images.githubusercontent.com/100426946/187731047-ff529c6f-1766-40a4-802b-03960c34c870.png)

COMANDO	DESCRIPCIÓN
docker build	Descripción. El comando docker build crea imágenes Docker a partir de un Dockerfile y un "contexto". El contexto de una compilación es el conjunto de archivos ubicados en la RUTA o URL especificada. El proceso de compilación puede hacer referencia a cualquiera de los archivos en el contexto. Por ejemplo, su compilación puede usar una instrucción COPY para hacer referencia a un archivo en el contexto...

# Descripción Para Los Comandos

![image](https://user-images.githubusercontent.com/100426946/187739072-3694f8d2-d28b-4ede-8d96-53056722f456.png)
![image](https://user-images.githubusercontent.com/100426946/187739152-4a3ac2b4-b06a-4a1f-bef6-d675e501b9c9.png)
![image](https://user-images.githubusercontent.com/100426946/187739245-f799891a-f06f-4285-bc65-9e8b32411613.png)

# Instalar el motor de Docker

Aunque en un principio Docker solo se usaba en las distribuciones de Linux, la versión actual del motor de contenedores se caracteriza por una gran independencia de plataforma. Hoy existen paquetes de instalación para Microsoft Windows y macOS, así como para servicios en la nube como Amazon Web Services (AWS)‎ y Microsoft Azur. Entre las distribuciones de Linux que soporta encontramos:

CentOS,
Debian,
Fedora,
Oracle Linux,
Red Hat Enterprise Linux,
Ubuntu,
openSUSE,
SUSE Linux Enterprise,

Además hay distribuciones de Docker gestionadas por la comunidad para:

Arch Linux,
CRUX Linux,
Gentoo Linux,

A continuación se muestra el proceso de instalación de un motor de Docker con Ubuntu, la popular distribución de Linux. Para conocer cómo instalar Docker en otras plataformas, accede a estas instrucciones de documentación de Docker en inglés.

Dependiendo de las exigencias y requisitos que se deben cumplir, puedes instalar Docker en el sistema Ubuntu de tres formas diferentes:

Manualmente con el paquete DEB
Desde el repositorio de Docker
Desde el repositorio de Ubuntu
Sin embargo, antes deberías de echar un vistazo a los requisitos del sistema del motor de Docker.

# Requerimientos de sistema

Para instalar la versión actual de Docker en la distribución de Ubuntu es necesaria la versión de 64 bits de una de las siguientes versiones de Ubuntu:

Yakkety 16.10,
Xenial 16.04 (LTS),
Trusty 14.04 (LTS).

Nota
En sistemas productivos se recomienda la instalación de productos de software con soporte a largo plazo (Long Term Support, LTS), pues de esta forma seguirán recibiendo actualizaciones aunque salgan nuevas versiones al mercado.

# Pasos previos para instalar Docker

En el siguiente tutorial de Docker se usa la versión UbuntuXenial 16.04 (LTS), aunque se pueden seguir los mismos pasos con Yakkety 16.10. Se recomienda a los usuarios de Trusty 14.04 (LTS) que antes de proceder a instalar Docker instalen los paqueteslinux-image-extra-*, ya que estos permiten que el motor de Docker tenga acceso al driver de almacenamiento AUFS.

# imagen de DOCKER
![WhatsApp Image 2022-09-15 at 4 43 48 PM](https://user-images.githubusercontent.com/100426946/190514821-ee042909-c518-4925-893e-6469138d238b.jpeg)

# MENU DE DOCKER
![image](https://user-images.githubusercontent.com/100426946/190516063-4c20d589-281e-4569-aec3-f861f3a01983.png)


# Crear Archivos DOCKER
Con Docker Compose podríamos crear un archivo de configuración en formato yaml y juntar los diferentes servicios y las opciones específicas para ejecutarlos de una sola vez. Como todos los cambios se almacenan en un archivo de configuración, la ejecución solo es aplicable a contenedores en un único host de Docker.
tambien cuando Cuando se usa una pila de aplicación LEMP, por ejemplo, con PHP, Nginx, MySQL y el framework de Laravel, Docker puede simplificar considerablemente el proceso de configuración.
se dice que la clave de la simplicidad en esta instalación es Docker Compose, que le permite crear un grupo de contenedores de Docker definidos en un solo archivo mediante un comando.

