# Validación — Texto degradado y luminosidad

## 27 de agosto de 2026

- La versión local confirma que el degradado se aplica al texto de ejemplo, no al fondo de la tarjeta.
- El selector de luminosidad ofrece Claro, Equilibrado y Oscuro; Metálico + Oscuro produjo un recorrido desde sombra ennegrecida hasta brillo controlado a partir de un color base.
- La primera comprobación de GitHub Pages mostró HTML actualizado con una versión previa de JavaScript/CSS por caché de archivos estáticos con el mismo nombre.
- Se añadieron parámetros de versión a `style.css` y `app.js` en `index.html` para que la siguiente publicación cargue los recursos actuales.

## Selector de tonos circulares

La siguiente versión sustituye el menú de luminosidad por una franja de cinco muestras circulares: Brillo, Claro, Equilibrado, Oscuro y Negro. Todas se calculan a partir del mismo color base. La muestra tipográfica elimina por completo el trazo exterior; el acabado Negro conserva un reflejo de material para que el texto no dependa de un borde blanco.

La comprobación final de GitHub Pages confirmó que la tira de cinco muestras circulares aparece en la herramienta publicada y que el texto de ejemplo usa el degradado directamente, sin contorno visible en el acabado Negro.

## Curvas de luz inspiradas en la referencia

La referencia aportada muestra una curva fría y oscura con tonos azulados a los extremos y una franja de brillo muy claro al centro. Se ajustaron los acabados de material para usar esa estructura visual: cinco puntos iniciales con sombra lateral, cuerpo intermedio, reflejo central, cuerpo intermedio y sombra final. El acabado Suave conserva dos paradas como valor base; los demás estilos abren con cinco para conservar su forma.
