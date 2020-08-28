# Flask

[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)

![Imgur](https://i.imgur.com/E3FqUTK.png?1)

[![Build Status](https://travis-ci.com/lderazo1/FInal2B.svg?branch=master)](https://travis-ci.com/lderazo1/FInal2B)

```{contents}
:depth: 2
```

## Descripción
Flask es un marco de aplicación web WSGI ligero . Está diseñado para que comenzar sea rápido y fácil, con la capacidad de escalar a aplicaciones complejas. Comenzó como una simple envoltura alrededor de Werkzeug y Jinja y se ha convertido en uno de los marcos de aplicaciones web Python más populares.

> Flask ofrece sugerencias, pero no impone ninguna dependencia o diseño del proyecto. Depende del desarrollador elegir las herramientas y bibliotecas que desea utilizar. La comunidad ofrece muchas extensiones que facilitan la adición de nuevas funciones.

## Instalación

Nos ubicamos en la terminal de nuestro Sistema Operativo y colocamos la siguiente sentencia.
```sh
pip install -U Flask
```
```{note}
Se recomienda el uso de entornos virtuales para el control de versiones de librerías en ejecución
```
## Métodos Utilizados
Algunos de los métodos que hemos utilizado se muestran a continuación:

| Función | Descripción |
| ------ | ------ |
| render_template () | Utilizado para renderizar plantillas. Como parámetros se proporciona el nombre de la plantilla y las variables que desea pasar al motor de templates como argumentos de palabras clave.|
| route() | URL que activar a las funciones |

## Demostración
Renderización de plantilla que primero fue ordenada por hora y fecha.
```sh
return render_template('report.html', reports = posts, courseName = posts[0]['courseName'], courseID = posts[0]['courseID'])
```
Renderización de plantilla ordenada por nombre de curso.
```sh
posts = sorted(posts, key=lambda post : post['courseName'])
return render_template('index.html', posts = posts, coursesTotal = len(posts))
```
