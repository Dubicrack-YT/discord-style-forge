# Discord Style Forge

Generador local y estático para crear nombres con Unicode para **roles**, **separadores**, **categorías** y **canales** de Discord. Incluye vista previa, botón de copiar, presets y paletas recomendadas por tipo de rol.

## Funciones

- Cuatro constructores: rol, separador, categoría y canal.
- Estilos Script, Fraktur, Gótico ancho y Limpio.
- Emojis sugeridos para canales de información, reglas, anuncios, verificación, soporte, multimedia, economía y staff.
- Paletas pensadas para roles de creador, miembro, verificación, edición, staff, identidad y edad.
- Generador de degradados CSS basado en **un solo color**: inicia en dos paradas de sombra y brillo, permite añadir hasta siete tonos claros, medios y oscuros, e incluye estilos suave, metálico, cromado, oro/mineral, aurora y mate.
- Selector de luminosidad **claro, equilibrado u oscuro** para que el mismo acabado pueda ir de un brillo blanco a un metal ennegrecido.
- Vista previa del **degradado aplicado al texto**, como una muestra de nombre de rol mejorado, sin colocar texto encima de un cuadro con degradado.
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
