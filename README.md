# Orden de batalla del Ejército Argentino

Presentación web con el orden de batalla del Ejército Argentino en simbología OTAN APP-6: estructura del CAAE, las tres divisiones de ejército y la Fuerza de Despliegue Rápido, mapa de guarniciones y anexo desplegado en PDF.

Funciona en cualquier navegador de escritorio, Android e iOS, y puede instalarse en la pantalla de inicio del teléfono.

## Contenido

| Archivo | Para qué sirve |
| --- | --- |
| `index.html` | La presentación completa: 5 diapositivas navegables más el mapa y las referencias, que se abren con sus botones en la barra inferior. Incluye estilos, tipografías y mapa; no necesita nada más. |
| `anexo_orden_de_batalla_EA.pdf` | Anexo con el orden de batalla totalmente desplegado, 10 páginas A4 apaisadas. |
| `logo-ea.png` | Isologotipo del Ejército Argentino que se muestra en la cabecera. |
| `manifest.webmanifest`, `sw.js`, `icon-*.png`, `apple-touch-icon.png` | Permiten instalarla como aplicación y consultarla sin conexión. |
| `.nojekyll` | Evita que GitHub Pages procese los archivos con Jekyll. |

## Publicar en GitHub Pages

1. Creá un repositorio nuevo en GitHub (puede ser público o privado con Pages habilitado según tu plan).
2. Subí todos los archivos de esta carpeta a la raíz del repositorio. Podés arrastrarlos en **Add file → Upload files** desde el navegador.
3. Entrá en **Settings → Pages**.
4. En **Source** elegí **Deploy from a branch**, rama `main` y carpeta `/ (root)`. Guardá.
5. Esperá un minuto. La dirección queda como `https://<usuario>.github.io/<repositorio>/`.
6. Abrí esa dirección en el teléfono. Conviene compartirla por QR o mensaje, no por archivo.

Todas las rutas son relativas, así que el sitio funciona igual en la raíz del dominio o dentro de un subdirectorio.

## Instalar en el teléfono

- **Android (Chrome):** abrí la dirección y tocá **Instalar aplicación** en el menú de tres puntos, o aceptá el aviso de instalación.
- **iOS (Safari):** tocá **Compartir → Agregar a inicio**. Safari solo permite instalar desde Safari, no desde Chrome ni desde otras aplicaciones.

Una vez instalada, se abre a pantalla completa y queda disponible sin conexión, incluido el anexo en PDF. Para actualizarla después de subir cambios, cerrala y volvé a abrirla dos veces, o subí `sw.js` con un número de versión nuevo en la constante `CACHE`.

## Mapa y referencias

Se abren desde los botones «Mapa» y «Referencias» de la barra inferior, y se cierran con el mismo botón, con «← Volver» o con la tecla Escape.

La vista «País» ubica sólo los comandos divisionarios (XX) y de brigada (X), y dibuja con recuadro punteado los cinco encuadres regionales: al tocar uno se amplía y aparecen todas las guarniciones de esa zona. El botón «Ampliar mapa», con el ícono de despliegue, agranda el mapa ocupando la diapositiva completa; se vuelve con el mismo botón o con la tecla Escape.

## Cabecera

La cabecera usa el isologotipo oficial sobre el color institucional `#242C4F`, el mismo que declara el sitio oficial del Ejército en argentina.gob.ar. Para cambiar el logotipo, reemplazá `logo-ea.png`; para cambiar el color, editá la variable `--ea` en el `<style>` de `index.html`.

## Notas sobre el contenido

- La composición proviene de las páginas oficiales de organización del Ejército (argentina.gob.ar), de 2018–2020, verificadas contra comunicados oficiales de 2026.
- Las guarniciones provienen del anexo «Organización del Ejército Argentino» de Wikipedia, basado en el Libro Blanco de la Defensa 2015. Las que no pudieron verificarse se marcan con «s/v» y marco discontinuo.
- Los regimientos argentinos de infantería y caballería tienen magnitud de batallón, por eso llevan escalón II.
- Toda la información proviene de fuentes abiertas.
