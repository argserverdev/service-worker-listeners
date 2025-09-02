# PWA Service Worker Listeners

Este es un proyecto de demostración de una Progressive Web App (PWA) que utiliza un Service Worker para interceptar y modificar peticiones de red.

## Descripción

El proyecto consiste en una página web simple que muestra una imagen. Sin embargo, un Service Worker intercepta la petición para esa imagen y la reemplaza por una imagen diferente.

Esto demuestra el poder de los Service Workers para controlar las peticiones de red y modificar las respuestas, lo que es una característica fundamental de las PWAs para habilitar funcionalidades offline y mejorar el rendimiento.

## Uso

Para ejecutar este proyecto, simplemente sirve los archivos en un servidor web local. No se requiere ninguna compilación o dependencia.

1.  Clona este repositorio.
2.  Inicia un servidor web en el directorio del proyecto. Por ejemplo, puedes usar `python -m http.server` o la extensión "Live Server" en Visual Studio Code.
3.  Abre tu navegador y navega a la dirección de tu servidor local (por ejemplo, `http://localhost:8000`).

Cuando la página cargue, verás que la imagen que se muestra es `main-patas-arriba.jpg` en lugar de `main.jpg`, gracias al Service Worker.

## Estructura de Archivos

```
.
├── css
│   └── style.css
├── img
│   ├── main-patas-arriba.jpg
│   └── main.jpg
├── js
│   └── app.js
├── .jshintrc
├── index.html
├── README.md
└── sw.js
```
