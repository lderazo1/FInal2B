# GUnicorn + Ngnix

[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)

![](https://pypi.org/static/images/logo-small.6eef541e.svg)

[![Build Status](https://travis-ci.com/lderazo1/FInal2B.svg?branch=master)](https://travis-ci.com/lderazo1/FInal2B)

```{contents}
:depth: 2
```

## Nginx
![Imgur](https://i.imgur.com/5MauW28.png?1)

Nginx está optimizado para todas las actividades de un servidor web, como por ejemplo:
  - Enrutar nombres de dominio (decide a dónde deben ir las solicitudes, o si una respuesta de error está en orden)
  - Servir archivos estáticos
  - Manejar muchas solicitudes que llegan a la vez
  - Manejar clientes lentos
  - Reenviar las solicitudes que deben ser dinámicas para Gunicorn
  - Manejar las peticiones https
  
Ejecutamos el servidor web nginx en localhost. Algunos de nuestros ejemplos se conectarán a scripts PHP en un servidor nginx que se ejecute localmente.
```sh
$ service nginx status
```
Salida
```
 * nginx is running
```

## GUnicorn
![Imgur](https://i.imgur.com/FtE3FFn.png?1)

Entre sus características se destaca
  - Ejecutar un grupo de procesos/subprocesos de trabajo
  - Traducir las solicitudes procedentes de Nginx (u otro servidor web) para que sean compatibles con WSGI
  - Llamar al código de Python cuando llega una solicitud
  - Traducir las respuestas WSGI de su aplicación en respuestas http adecuadas

## WSGI

WSGI es la interfaz de puerta de enlace del servidor web. Es una especificación que describe cómo un servidor web se comunica con las aplicaciones web y cómo las aplicaciones web se pueden encadenar para procesar una solicitud. Un componente de middleware WSGI es un Python invocable que es en sí mismo una aplicación WSGI. Un componente WSGI puede realizar funciones como:

## Implementación y resultados

### Reportes

```{image} images/esquema.png
---
scale: 40
---
```
Esquema Reporte

```{image} images/reporte.png
---
scale: 40
---
```
Registro de Reportes

```{image} images/pagina.png
---

scale: 40
---
```
Lista de Reportes
```
