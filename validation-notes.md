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

La validación local de Metálico con el color base `#C77DFF` produjo cinco paradas diferenciadas: `#4A1770` → `#AE4DF7` → `#F3EBF9` → `#B562F4` → `#4A1770`. El commit de publicación ya fue registrado; durante la primera consulta posterior, GitHub Pages aún mostraba el despliegue anterior, por lo que queda pendiente confirmar su propagación final.

La publicación final se verificó en GitHub Pages: Metálico abre con cinco bandas, incluyendo sombra morada profunda en ambos extremos, transición fría en el cuerpo y un brillo central claro. La curva ya no es una rampa lineal de claro a oscuro.

## Selector simplificado de color

La siguiente revisión sustituye las cinco muestras de luminosidad por tres muestras: Oscuro, Equilibrado y Claro. El control se compacta en una sola franja azul con círculos, aro blanco y un símbolo visual de cuentagotas, siguiendo la composición de la referencia. Los tres tonos se derivan del color base, pero el fondo azul de la franja se mantiene estable para que el control tenga una identidad visual clara.

La comprobación local confirmó que el control muestra exactamente tres muestras y que Oscuro actualiza la salida usando el color base y una sombra más profunda, manteniendo la barra azul compacta y la vista de texto sin contorno.

GitHub Pages confirmó el despliegue de la revisión del selector simplificado el 27 de agosto de 2026 a las 22:08. La fuente de publicación sigue siendo la rama `main` y la carpeta raíz.

La comprobación visual de la publicación confirmó que el generador muestra la barra azul compacta con tres círculos de selección y sus símbolos claros. El orden visible es Oscuro, Equilibrado y Claro, sin la paleta anterior de cinco niveles.

## Corrección de la salida de colores

La versión siguiente elimina las cápsulas rectangulares que mostraban hexadecimal y porcentaje para cada banda. En ambos lugares de salida, los colores generados se representan ahora como círculos con aro blanco dentro de una franja azul compacta, sin exponer texto de valores junto a cada muestra.

## Reinterpretación tonal de referencia

La referencia no describe cinco aclarados del mismo color. Su lectura visual es asimétrica: primer tono cian saturado, segundo azul hielo, tercero blanco con matiz frío, cuarto grafito casi negro y quinto azul marino. El modo Metálico ahora usa esa relación como su receta por defecto y abre con el color base cian `#16B8E9`; el selector sigue permitiendo una sola entrada de color para derivar variaciones.
