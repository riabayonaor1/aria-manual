# Fuentes y alcance del manual ARIA

Edición 01 — 16 de octubre de 2026, Colombia.

Este resumen identifica las fuentes locales consultadas en el proyecto. Los originales permanecen en el espacio de trabajo; no se publica el software privado del robot ni sus configuraciones, credenciales o registros completos.

## Documentación primaria del proyecto

- `aria_raspberry/LEEME.md`: arquitectura, activación por nombre, ventana de conversación, audio, rostro, modelos configurados, servicio y habilidades.
- `aria_raspberry/CNC_OPERACION_POR_VOZ.md`, actualización del 14 de octubre: referencia física Z, medición, origen, borde, montaje del lápiz y cancelación.
- `aria_raspberry/CNC_TEXTO_DIBUJOS_FUNCIONES.md`: texto, biblioteca, dibujo generado, vectorización, funciones, formatos y límites.
- `aria_raspberry/MOVIL.md`: micrófono remoto, HTTPS local, certificado, sesión y cancelación.
- `work/aria_alarm9_20261014/final-validation.json`: estado y perfil del firmware `20261014-ARIA-LIMITS-R6`, recorrido medido y pruebas en seco.
- `work/aria_alarm9_20261014/measurement-r6-validation.json`: medición aceptada, área guardada y finalización Idle en esa sesión.
- `work/aria_alarm9_20261014/firmware_r6/VALIDATION.md`: firmware y finales de carrera.
- `output/sustentacion_aria_2026-10-15/Fuentes_ARIA.md`: procedencia del CAD, modelo Uno R3, atribuciones y alcance de la demostración.

## Qué consta

Raspberry Pi 4B, Uno R3, tres motores 28BYJ-48 de 5 V y drivers ULN2003; rostro OLED SSD1306; Python; Vosk; OpenAI para transcripción y conversación; ElevenLabs para voz. La instalación documenta activación local y control CNC con validación de referencias, área y límites.

Recorrido registrado: 61,699 × 72,488 mm. Con margen de 3 mm, área interior 55,699 × 66,488 mm. Medir recorrido no calibra por sí mismo la escala pasos/mm.

Los registros acreditan pruebas de software, interpretación, conversión y movimiento sin lápiz. El perfil indica `dry_run_without_pen: true` y contacto con papel no confirmado. Las vistas y los archivos generados no prueban escritura física ni precisión dimensional. El manual describe la capacidad implementada y las comprobaciones que aún exige el montaje real.

## Material visual

El GLB del visor procede del ensamblaje CNC de Autodesk Fusion con adaptación de la electrónica a Uno R3: 316 mallas, 18 grupos, 96.030 triángulos. El modelo se presenta con materiales grafito y salvia y contornos añadidos. La posición de la electrónica y el despiece son explicativos.

- Mecánica: Simple CNC Plotter de mith, https://www.thingiverse.com/thing:4796222, derivado de DAZ, https://www.thingiverse.com/thing:4579436. Creative Commons Attribution según el paquete original; no se atribuye una versión no documentada.
- Uno R3: benjamino, https://www.cadcrowd.com/3d-models/arduino-uno, CC BY 4.0, https://creativecommons.org/licenses/by/4.0/. Adaptaciones: empaquetado GLB, orientación y materiales.
- Three.js: MIT; licencia conservada en assets/vendor/THREE-LICENSE.txt.
- Tipografías: Architects Daughter, DM Sans e IBM Plex Mono, SIL OFL; archivos y licencias conservados en assets/fonts/.
- Ilustraciones isométricas originales creadas para el manual: Raspberry Pi 4B, Arduino Uno R3 y motor 28BYJ-48 con ULN2003.

El manual no contiene código de acceso móvil, claves API ni certificados privados. El QR enlaza únicamente al manual público en GitHub Pages.

## Identidad oficial ARIA

Se reutiliza sin rediseñar el logo oficial de la presentación del proyecto, confirmado por el usuario el 16 de octubre de 2026: https://riabayonaor1.github.io/aria-presentacion/inmersiva/#video. Se conserva su forma y color en cabecera, pie e icono del sitio.
