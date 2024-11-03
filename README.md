# README - PPS Unidad 0 Actividad 3

## Índice

1. [Introducción](./README.md#1-introducción)
2. [Instalación de KeePass2 en el equipo Windows](./README.md#2-instalación-de-keepass2-en-el-equipo-windows)  
3. [Principales funcionalidades de KeePass2](./README.md#3-principales-funcionalidades-de-keepass2)

4. [Creación de una Base de Datos de Contraseñas](./GitHub.md#1-funciones-básicas-de-github)
   - [Funciones Básicas](./GitHub.md#Funciones-Básicas-de-GitHub)
     - [Crear una Cuenta en GitHub](./GitHub.md#)
     - [Iniciar sesión en la cuenta de GitHub](./GitHub.md#-1)
     - [Crear un Repositorio](./GitHub.md#-2)
     - [Clonar un Repositorio](./GitHub.md#-3)
     - [Subir Archivos a un Repositorio](./GitHub.md#-4)
     - [Crear y Gestionar Issues](./GitHub.md#-5)
     - [Crear un Pull Request](./GitHub.md#-6)
     - [Revisar y Aceptar Pull Requests](./GitHub.md#-7)
     - [Configuración de Claves SSH](./GitHub.md#-8)
   - [Ejemplos prácticos y capturas](./GitHub.md#2-capturas-y-ejemplos)

5. [Sincronización con la Nube](#contenidos-del-repositorio)
6. [Instalación de KeePass2 en el Dispositivo Móvil]()

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

1. **Creación y Gestión de Bases de Datos de Contraseñas**:
   - KeePass2 permite la creación de bases de datos cifradas donde se almacenan todas tus contraseñas. Estas bases de datos están protegidas mediante un algoritmo de cifrado avanzado (AES-256).
   - Para crear una nueva base de datos, ve a **Archivo** > **Nuevo** y sigue los pasos para configurar una contraseña maestra que protegerá todos los datos almacenados.
<p align="center">
  <img src="./images/Crear%20Database.png" alt="Descargar keepass en pc">
</p>
<p align="center"><em>Imagen 2: Crear una base de datos</em></p>

<p align="center">
  <img src="./images/Crear%20contraseña%20maestra.png" alt="Crear contraseña maestra">
</p>
<p align="center"><em>Imagen 3: Crear contraseña maestra</em></p>

2. **Organización en Grupos y Categorías**:
   - La aplicación permite organizar las contraseñas en grupos o categorías para facilitar su acceso y gestión. Por ejemplo, puedes crear grupos separados para *trabajo*, *personal*, *bancos*, *redes sociales*, etc.

<p align="center">
  <img src="./images/Organizacion%20categorias%20contraseñas.png" alt="Organizacion categorias contraseñas">
</p>
<p align="center"><em>Imagen 4: Organizacion de categorias y contraseñas de una base de datos</em></p>

3. **Generador de Contraseñas Seguras**:
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

4. **Sincronización, Copia de Seguridad y exportación de las BBDD**:

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

   - asdfg
