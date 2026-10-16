# ARIA · Manual de usuario

Manual web en español sobre la construcción, tecnologías y uso del asistente ARIA y su CNC de escritura. Estética de boceto arquitectónico, ilustraciones vectoriales originales y modelo 3D interactivo del proyecto.

- **Manual público:** https://riabayonaor1.github.io/aria-manual/
- **Sites:** https://aria-manual-de-usuario.rickynovich32.chatgpt.site (acceso de su propietario)
- **QR PNG:** [descargar](dist/assets/qr-manual.png)
- **QR SVG:** [descargar](dist/assets/qr-manual.svg)

## Consultar y usar

Navega por el índice; busca con el botón de búsqueda o la tecla `/`. Filtra los ejemplos por función, abre las preguntas de ayuda y usa «Imprimir / guardar PDF» para obtener una copia completa. El visor permite girar, seleccionar, enfocar motores/controlador y mostrar un despiece explicativo. Conserva una imagen si WebGL 2 no está disponible.

La página es un manual estático: no se conecta al robot ni recibe credenciales. El control real requiere la interfaz local de la Raspberry en su propia red.

## Ejecutar localmente

Desde este directorio:

```sh
python3 -m http.server 8793 --directory dist --bind 127.0.0.1
```

Abrir http://127.0.0.1:8793/. No requiere instalar paquetes ni construir. Los archivos de tipografía, visor, modelo e ilustraciones se sirven localmente.

## Publicación

`.github/workflows/pages.yml` publica `dist/` al actualizar `main`. GitHub Pages debe estar configurado con origen GitHub Actions. La misma carpeta se publica en Sites usando la configuración `.openai/hosting.json`. Los recursos usan rutas relativas para funcionar bajo `/aria-manual/`.

## Edición y evidencia

Edición 01, 16 de octubre de 2026. Las funciones se documentaron a partir del software de ARIA y los registros R6 del 14 de octubre. Las pruebas acreditan conversión y movimiento sin lápiz; el contacto y la calidad de escritura sobre papel requieren validación física. Las dimensiones corresponden a ese montaje y no garantizan precisión.

Ver [fuentes y alcance](dist/FUENTES.html) y [resumen de evidencia](dist/EVIDENCIA.md).

## Créditos y licencias

- Mecánica basada en Simple CNC Plotter de **mith**, derivada de DAZ; licencia Creative Commons Attribution según el archivo original conservado en `dist/assets/model/MECANICA-LICENSE.txt`.
- Arduino Uno de **benjamino / Cad Crowd**, CC BY 4.0. Ver `dist/assets/model/UNO_FUENTE_Y_LICENCIA.md`.
- Three.js, MIT: `dist/assets/vendor/THREE-LICENSE.txt`.
- Architects Daughter, DM Sans e IBM Plex Mono, SIL OFL: licencias en `dist/assets/fonts/`.
- Se conserva el logo oficial de ARIA de la presentación del proyecto, sin rediseñarlo.
- Las ilustraciones SVG y el diseño del manual fueron creados para el proyecto ARIA. La imagen de referencia aportada solo orientó la estética y no se redistribuye.
