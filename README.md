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
![flujo](https://user-images.githubusercontent.com/100426946/187731047-ff529c6f-1766-40a4-802b-03960c34c870.png)

