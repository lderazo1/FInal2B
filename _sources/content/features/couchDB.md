# CouchDB

[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)

![Imgur](https://i.imgur.com/QIqqSen.png)
[![Build Status](https://travis-ci.com/lderazo1/FInal2B.svg?branch=master)](https://travis-ci.com/lderazo1/FInal2B)
## Descripción

Apache CouchDB es uno de los nuevos sistemas de gestión de bases de datos. Su arquitectura interna es tolerante a fallas, y las fallas ocurren en un ambiente controlado y se tratan con elegancia. Los problemas individuales no se propagan en cascada a través de un sistema de servidor completo, sino que permanecen aislados en solicitudes únicas.
Creemos que CouchDB cambia drásticamente la forma en que crea aplicaciones basadas en documentos. CouchDB combina un modelo de almacenamiento de documentos intuitivo con un potente motor de consultas de una manera simple.

## Instalación (Linux)
1. Actualizar el repositorio local del administrador de paquetes apt
```sh
$ sudo apt-get update
```
2. Actualizar los paquetes del sistema
```sh
$ sudo apt-get upgrade
```
3. Instalación de paquete para la gestión sencilla de repositorios
```sh
$ sudo apt-get install software-properties-common
```
4. Añadir repositorio CouchDB-PPA
```sh
$ sudo add-apt-repository ppa:couchdb/stable
```
5. Actualizar nuevamente el repositorio local del administrador de paquetes apt ya que se ha agregado un nuevo repositorio
```sh
$ sudo apt-get update
```
6. Instalar CouchDB con las dependencias requeridas
```sh
$ sudo apt-get install couchdb
```
```{Note}
Se muestra una interfaz donde se les solicitará la configuración inicial, recomendable standalone que es para realizar una configuración del servidor independiente.
```
## Comandos

Algunos comandos básicos de manejo en CouchDB

| Comando | Descripción |
| ------ | ------ |
| sudo service couchdb start | Permite iniciar los servicios de la base de datos |
| sudo service couchdb stop | Permite detener los servicios de la base de datos |
| sudo service couchdb status | Permite conocer el estado de los servicios de la base de datos |

## Acceso

Ejecutar http://dominio:5984/_utils/
```{Note}
reemplezar dominio por el dominio establecido en la configuración inicial, para fines practicos se optó por 127.0.0.1
```
## DataTable
Toma una tabla HTML existente y le agrega funcionalidad. También puede extraer datos de un JSON remoto y crear tablas sobre la marcha. Es una característica útil. Aunque para grandes conjuntos de datos no funciona, ya que todo el conjunto de datos se extrae de una vez. Para tales conjuntos de datos, DataTable admite el procesamiento del lado del servidor.

## Vistas
Algunos propósitos de las vistas son los siguientes
* Filtrar los documentos en su base de datos para encontrar aquellos relevantes para un proceso en particular.
* Extraer datos de sus documentos y presentarlos en un orden específico.
* Creación de índices eficientes para buscar documentos por cualquier valor o estructura que resida en ellos.
* Utilice estos índices para representar relaciones entre documentos.
* Finalmente, con vistas puede hacer todo tipo de cálculos sobre los datos en sus documentos. Por ejemplo, si los documentos representan las transacciones financieras de su empresa, una vista puede responder a la pregunta de cuál fue el gasto en la última semana, mes o año.
