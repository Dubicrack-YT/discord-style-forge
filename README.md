# Discord Style Forge

Generador local y estático para crear nombres con Unicode para **roles**, **separadores**, **categorías** y **canales** de Discord. Incluye vista previa, botón de copiar, presets y paletas recomendadas por tipo de rol.

## Funciones

- Cuatro constructores: rol, separador, categoría y canal.
- Estilos Script, Fraktur, Gótico ancho y Limpio.
- Emojis sugeridos para canales de información, reglas, anuncios, verificación, soporte, multimedia, economía y staff.
- Paletas pensadas para roles de creador, miembro, verificación, edición, staff, identidad y edad.
- Generador de degradados CSS basado en **un solo color**: inicia en dos paradas de sombra y brillo, permite añadir hasta siete tonos claros, medios y oscuros, e incluye estilos suave, metálico, cromado, oro/mineral, aurora y mate.
- Los estilos de material usan una curva de varios puntos: **sombra lateral → tono medio → brillo central → tono medio → sombra lateral**. Por ello, al seleccionar un acabado metálico, cromado, oro, aurora o mate se proponen cinco paradas; Suave mantiene dos por defecto.
- El acabado metálico predeterminado interpreta una progresión fría de cinco tonos: **cian vivo → azul hielo → blanco azulado → grafito → azul marino**. El selector de color base permite desplazar ese material a otra familia de color sin volverlo una rampa lineal.
- Franja azul compacta de **tres muestras circulares** para elegir Oscuro, Equilibrado o Claro desde el mismo color base, inspirada en el formato visual de la referencia y no en un menú desplegable.
- Las bandas de salida se muestran como una franja de **círculos de color**, sin cápsulas de hexadecimal ni porcentajes, para que el resultado visual siga el mismo formato de selección.
- Vista previa del **degradado aplicado al texto**, como una muestra de nombre de rol mejorado; los acabados oscuros se muestran sin borde ni contorno.
- Presets inspirados en 『 Dubicrack Community 』 sin conexión a la API de Discord.
- Todo se procesa en el navegador; no se solicita inicio de sesión ni se guardan textos.

## Uso

Abre `index.html` en tu navegador o visita el sitio publicado. Elige el tipo de elemento, escribe el texto, selecciona el estilo y copia el resultado. En roles, elige primero la función del rol para ver una paleta recomendada; los colores de identidad no deben conceder permisos por sí mismos. En Degradados, elige el color base, el acabado y la luminosidad: todas las paradas se calculan automáticamente sin pedir colores secundarios. La muestra deja el degradado dentro del texto para imitar un nombre de rol mejorado. El CSS generado sirve para fondos, embeds o referencias visuales; los colores normales de rol en Discord siguen siendo planos.

## Desarrollo y publicación

El proyecto no requiere dependencias ni build.

```bash
python3 -m http.server 4173
```

GitHub Pages se publica desde la rama `main` mediante el flujo incluido en `.github/workflows/deploy-pages.yml`.

## Licencia

MIT. Consulta [LICENSE](LICENSE).
