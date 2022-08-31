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

![image](https://user-images.githubusercontent.com/100426946/187739072-3694f8d2-d28b-4ede-8d96-53056722f456.png)
![image](https://user-images.githubusercontent.com/100426946/187739152-4a3ac2b4-b06a-4a1f-bef6-d675e501b9c9.png)
![image](https://user-images.githubusercontent.com/100426946/187739245-f799891a-f06f-4285-bc65-9e8b32411613.png)

# Descripción Para Los Comandos
