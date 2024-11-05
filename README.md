# README - PPS Unidad 0 Actividad 3

## Índice

1. [Introducción](./README.md#1-introducción)
2. [Instalación de KeePass2 en el equipo Windows](./README.md#2-instalación-de-keepass2-en-el-equipo-windows)  
3. [Principales funcionalidades de KeePass2](./README.md#3-principales-funcionalidades-de-keepass2)
   - [Creación y Gestión de Bases de Datos de Contraseñas](#1-creación-y-gestión-de-bases-de-datos-de-contraseñas)
   - [Organización en Grupos y Categorías](#2-organización-en-grupos-y-categorías)
   - [Generador de Contraseñas Seguras](#3-generador-de-contraseñas-seguras)
   - [Sincronización, Copia de Seguridad y exportación de las BBDD](#4-sincronización-copia-de-seguridad-y-exportación-de-las-bbdd)
   - [Aplicación para teléfono móvil](#5-aplicación-para-teléfono-móvil)

---

## 1. Introducción
En esta tarea, trabajaremos con KeePass2, un gestor de contraseñas de código abierto que permite almacenar y gestionar de forma segura las credenciales de acceso. A lo largo de esta práctica, aprenderemos a instalar y configurar KeePass2 en un equipo, añadir paquetes de idioma, crear una base de datos de contraseñas, y explorar la integración de plugins para sincronizar datos con servicios en la nube. A mayores, se probará esa sincronización en la nube con otro dispositivo, como un dispositivo móvil. Finalmente, se documentará el proceso en un archivo Markdown que incluirá los pasos seguidos y los resultados obtenidos.

El objetivo de esta práctica es familiarizarnos con el uso de KeePass2 y su funcionamiento en distintos dispositivos, así como entender cómo se pueden gestionar de manera segura las contraseñas en un entorno local y sincronizado con la nube.


## 2. Instalación de KeePass2 en el equipo Windows
Para comenzar a trabajar con KeePass2, es necesario descargar e instalar la aplicación en el equipo. En este caso, utilizaremos un sistema operativo Windows, puesto que en Linux no funcionan los plugins de sincronización con la nube.

1. **Accede a la página oficial de KeePass2:**
   - Dirígete a la página oficial de [KeePass](https://keepass.info/download.html) para acceder a la última versión disponible de **KeePass2** y garantizar la descarga desde una fuente segura.
2. **Seleccione la versión correcta:**
   - En la sección de descargas, selecciona la versión de KeePass2 adecuada para tu sistema operativo (Windows, Linux o macOS). En nuestro caso, elegiremos Windows. 
   - Asegúrate de descargar la versión completa y no solo el archivo portátil si prefieres la instalación tradicional.

<p align="center">
  <img src="./images/Descargar%20keepass%20en%20pc.png" alt="Descargar keepass en pc">
</p>
<p align="center"><em>Imagen 1: Descargar keepass en pc</em></p>

3. **Proceso de Instalación:**
   - Una vez descargado el instalador, haz doble clic en el archivo descargado para comenzar la instalación.
   - Completa la instalación haciendo clic en “Instalar” y luego en “Finalizar” una vez que el proceso haya concluido


## 3. Principales funcionalidades de KeePass2
KeePass2 es un gestor de contraseñas seguro y de código abierto que permite gestionar y almacenar contraseñas de manera eficiente. A continuación, se describen las funcionalidades más destacadas de la aplicación y cómo pueden ser utilizadas para gestionar tus credenciales de forma segura.

##### 1. **Creación y Gestión de Bases de Datos de Contraseñas**:
   - KeePass2 permite la creación de bases de datos cifradas donde se almacenan todas tus contraseñas. Estas bases de datos están protegidas mediante un algoritmo de cifrado avanzado (AES-256).
   - Para crear una nueva base de datos, ve a **Archivo** > **Nuevo** y sigue los pasos para configurar una contraseña maestra que protegerá todos los datos almacenados.
<p align="center">
  <img src="./images/Crear Database.png" alt="Descargar keepass en pc">
</p>
<p align="center"><em>Imagen 2: Crear una base de datos</em></p>

<p align="center">
  <img src="./images/Crear%20contraseña%20maestra.png" alt="Crear contraseña maestra">
</p>
<p align="center"><em>Imagen 3: Crear contraseña maestra</em></p>

##### 2. **Organización en Grupos y Categorías**:
   - La aplicación permite organizar las contraseñas en grupos o categorías para facilitar su acceso y gestión. Por ejemplo, puedes crear grupos separados para *trabajo*, *personal*, *bancos*, *redes sociales*, etc.

<p align="center">
  <img src="./images/Organizacion%20categorias%20contraseñas.png" alt="Organizacion categorias contraseñas">
</p>
<p align="center"><em>Imagen 4: Organizacion de categorias y contraseñas de una base de datos</em></p>

##### 3. **Generador de Contraseñas Seguras**:
   - KeePass2 incluye una herramienta de generación de contraseñas seguras y personalizables. Esta función es útil para crear contraseñas complejas que aumenten la seguridad de tus cuentas.
   - Cada vez que se vaya a introducir una *key* en la BBDD se generará una contraseña con este generador, cuyos valores se puede modificar para generar contraseñas más complejas (como son como introducir carácteres en específico o un mayor número de caracteres) o directamente poner una contraseña que nosotros deseemos.
<p align="center">
  <img src="./images/Generar%20key.png" alt="Generar una key">
</p>
<p align="center"><em>Imagen 5: Generar una key</em></p>

<p align="center">
  <img src="./images/Parametros%20generador%20de%20contraseña.png" alt="Parámetros del generador de contraseñas">
</p>
<p align="center"><em>Imagen 6: Parámetros del generador de contraseñas</em></p>

##### 4. **Sincronización, Copia de Seguridad y exportación de las BBDD**:

KeePass2 permite sincronizar bases de datos con servicios en la nube usando plugins. Esta función es útil si necesitas acceder a tus contraseñas desde múltiples dispositivos. Plugins como **KeeAnywhere** facilitan la integración con servicios de almacenamiento en la nube como Google Drive, Dropbox, y OneDrive. 

Ésto puede ser muy útil para tener las contraseñas en distintos dispositivos, puesto que se crean copias de seguridad en la nube para ello. La sincronización permitiría que los cambios realizados en un dispositivo se traspasen a la copia en la nube y, por ende, al resto de dispositivos.

Tambien se pueden exportar los datos en formatos como CSV, XML, o KDBX para tener un respaldo de los archivos en caso de que se perdiesen.

A continuación, se especificarán los pasos a seguir para conseguir todo esto:
   - Para realizar la exportación en un formato deseado ve a **Archivo** > **Exportar**.
   - Para conseguir la integración con servicios de almacenamiento en la nube descargaremos el plugin **KeeAnywhere**. Dirígete a la página oficial de [KeeAnywhere](https://keeanywhere.de/) para descargar el archivo.
<p align="center">
  <img src="./images/Descargar%20plugin.png" alt="Descargar plugin de integración con la nube">
</p>
<p align="center"><em>Imagen 7: Descargar plugin de integración con la nube</em></p>

   - Una vez descargado, debemos introducir el archivo (que será un .plgx) en la carpeta **Plugins** de la aplicación. Para ello debemos dirigirnos a la carpeta donde tengamos el programa instalado.
<p align="center">
  <img src="./images/añadir%20plugin%20en%20la%20carpeta%20de%20plugin.png" alt="Configurar archivo de plugin en la carpeta correspondiente">
</p>
<p align="center"><em>Imagen 8: Configurar archivo de plugin en la carpeta correspondiente</em></p>

   - Una vez integrado el plugin en la carpeta, debemos reiniciar la aplicación y, en *herramientas*, nos aparecerá una opción para el plugin. En nuestro caso elegiremos el caso de Google Drive Restricted, que es la opción con la que mejor trabaja el plugin.
<p align="center">
  <img src="./images/Opcion%20plugin.png" alt="Elegir opción con la herramienta del plugin">
</p>
<p align="center"><em>Imagen 9: Elegir opción con la herramienta del plugin</em></p>

   - Una vez seleccionada no saldrá un desplegable en el buscador para iniciar sesión con google. Aquí introducimos nuestra cuenta para poder conectarnos con la nube
<p align="center">
  <img src="./images/Opcion%20plugin.png" alt="Elegir opción con la herramienta del plugin">
</p>
<p align="center"><em>Imagen 10: Introducir cuenta para Google Drive</em></p>

   - Una vez introducida la cuenta tenemos 2 métodos de guardado. 
     - *Guardar en url*: es una opción en la que directamente la base de datos se conecta a la nube, por lo que siempre estará en la nube y necesitas siempre internet para conectarte a ella
     - *Guardar copia en la nube*: esta opción es la que escogeremos, puesto que guarda una copia de nuestra base en la nube, así podemos acceder a nuestras contraseña sin wifi y tendremos la copia de respaldo en la nube. Para utilizar esta opción, vamos a **Archivo** > **Guardar como** > **Guardar copia en la nube**. Nos saldrá una herramienta en la que podremos navegar sobre carpeta (solo carpeta y archivos .kdbx) para guarda la copia donde deseemos. En *filename* debemos ponerle un nombre identificativo a la copia, distinto a la que tenemos en el programa. 
> ⚠️ **NOTA:** Copiamos la URL donde guardamos la copia para el siguiente paso, para poder hacer la sincronización. La URL debe ser con el propio archivo incluido dentro, no solo con la carpeta.
<p align="center">
  <img src="./images/Guardar%20copia%20nube.png" alt="Guardar una copia en la nube">
</p>
<p align="center"><em>Imagen 11: Guardar una copia en la nube</em></p>

   - Por último, para que los cambios que hagamos en local se hagan efectivos en la copia de la nube y viceversa, debemos activar la sincronización. Con la url de la copia nos dirigimos a **Archivo** > **Sincronizar** > **Guardar copia en la nube**. Aquí debemos introducir la URL hacia la copia y las credenciales de la cuenta en la que está alojada la copia. Es mejor seleccionar la opción de recordar usuario y contraseña para que no esté pidiendolos constantemente, ademas éstas se guardan en un fichero encriptado, por lo que solo nosotros las conocemos.
<p align="center">
  <img src="./images/Activar%20sincronizacion.png" alt="Activar Sincronización">
</p>
<p align="center"><em>Imagen 12: Activar Sincronización</em></p>

##### 5. Aplicación para teléfono móvil
Como tenemos realizada toda la configuración con la nube, podemos compartir las bases de datos con otros dispositivos, por ejemplo un teléfono movil. En Android, la aplicación está en Google Play Store. Una vez descargada la aplicación solo hay que dar a la pestaña abrir archivo. Se desplegará el inicio de sesión con la cuenta que deseemos (en nuestro caso de Google). Seleccionamos la base de datos que se deese abir. Introduce la clave maestra de la base de datos y tendrá acceso a ella.
<p align="center">
  <img src="./images/inicio%20en%20movil.jpg" alt="Activar Sincronización">
</p>
<p align="center"><em>Imagen 13: Aplicación para Android</em></p>

<p align="center">
  <img src="./images/seleccionar%20archivo%20en%20movil.jpg" alt="Seleccionar base de datos">
</p>
<p align="center"><em>Imagen 14: Seleccionar base de datos</em></p>

<p align="center">
  <img src="./images/cuentas%20en%20movil.jpg" alt="Cuentas y contraseñas desde el móvil">
</p>
<p align="center"><em>Imagen 15: Cuentas y contraseñas desde el móvil</em></p>