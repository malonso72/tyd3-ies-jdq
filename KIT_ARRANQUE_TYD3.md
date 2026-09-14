# Kit de arranque · TyD 3º ESO (tyd3-ies-jdq)

Última actualización: septiembre 2026
Mantenedor: Manuel Alonso Herrera (malonso72@gmail.com)
Repositorio: github.com/malonso72/tyd3-ies-jdq
Web en vivo: https://tyd3-ies-jdq.malonso72.workers.dev

---

## Quién soy y qué hago aquí

- Profesor de Tecnología y Digitalización en el IES Jiménez de Quesada (Santa Fe, Granada).
- Esta es la web docente del curso **Tecnología y Digitalización · 3º ESO**.
- Cloudflare Workers (Static Assets). `git push` a `main` despliega solo (integración con GitHub); el hook de pre-push verifica HTML y enlaces antes.

## Las 6 unidades del curso

- `01-dibujo-tecnico` — Dibujo técnico
- `02-construccion-objetos` — Construcción de objetos
- `03-redes-comunicaciones` — Redes y comunicaciones
- `04-mecanismos-motores` — Mecanismos y motores
- `05-circuitos-robotica` — Circuitos y robótica (incluye mixtos, electrónica, Arduino)
- `06-programacion-ia` — Programación e IA

## Otros repos que llevo

Si te pido tocar algo de OTRO curso, no es este repo. Dilo y abrimos otro chat.

- `tyd2-ies-jdq` — Tecnología y Digitalización · 2º ESO (tiene KIT_ARRANQUE_TYD2.md)
- `tec4-ies-jdq` — Tecnología · 4º ESO (tiene KIT_ARRANQUE_TEC4.md)
- `cyr1-ies-jdq` — Computación y Robótica · 1º ESO
- `teci2-ies-jdq` — Tecnología e Ingeniería II · 2º Bachillerato (tiene KIT_ARRANQUE_TECI.md)
- `tecnologia-ies-jdq` — hub general

## Tono y forma de trabajar

- Español, conciso, sin verborrea.
- No uses emojis salvo que yo los use primero.
- Cambio en varios pasos → primero RECAP de lo entendido y espera mi OK antes de tocar nada.
- Cambio claro y autocontenido → hazlo y resumes al final.
- El push lo decido yo: tú haces commit y me preguntas antes de hacer push (despliega a la web que usan los alumnos).
- A veces se cuelga `.git/index.lock` y bloquea commits desde GitHub Desktop. Hay que borrarlo del disco.
- Antes de cambios grandes deja backup con sufijo `.bak_<descripcion>`.

## Decisiones que NO hay que rediscutir

### Estructura del libro digital de cada unidad

Mismo patrón que en TyD 2º:
- `unidades/0X-nombre/libro-digital.html` con `const banco = { 1: {...}, ..., N: {...} }` y `const imgs = {...}`.
- LaTeX MathJax con `\\[ ... \\]` en `teoria_html`.
- Imágenes EMBEBIDAS como data URLs (autocontenido).
- Esquemas vectoriales → SVG inline con `width` y `height` EXPLÍCITOS y subíndices con `<tspan>` (NO uses caracteres Unicode ₁ ₂ ₜ — fallan con algunos fonts).

### Unidad 5 · Circuitos y robótica

Esta unidad fue REVAMPADA respecto a la versión de 2º:
- Hub renombrado a "**Circuitos y robótica**" (no solo electricidad).
- Incluye **circuitos mixtos** (serie+paralelo combinados), electrónica básica y bloque Arduino.
- En PARALELO uso la fórmula **producto entre suma** (R_eq = R₁·R₂/(R₁+R₂)). La general SOLO aparece en la teoría junto con la del producto entre suma; en los ejercicios solo la del producto entre suma.
- Llamo "**R_eq**" (resistencia equivalente), NO R_t. La teoría menciona "también llamada total" para alumnos con esa terminología.
- Hay interactivos:
  - Calculadora de circuitos mixtos
  - Identificador de componentes
  - Arduino blink

### Exámenes (cuando te pida uno)

Esquema por defecto (mismo que TyD 2º) salvo que te diga otra cosa:
- Word `.docx` para alumno + solucionario aparte.
- Cabecera con datos del alumno + caja "NOTA __/10".
- **Teoría tipo test**, 4 opciones, cuadradito ☐ delante. Sin penalización.
- **Ejercicios** con cálculos, espacio en blanco con borde inferior.
- Solucionario en VERDE con paso a paso.
- Tensión por defecto: 12 V (números redondos).

## Estado (septiembre 2026)

Las 6 unidades completas: hub, libro digital, interactivos, actividades (U4 con el cuadernillo de 64
ejercicios integrado), autocomprobación y proyecto. U1 Dibujo técnico comparte libro, simuladores y
láminas con 2.º y 4.º (misma unidad progresiva). Enlaces de repaso a TyD 2.º en los hubs, verificados.

Pasada de limpieza de septiembre de 2026 (misma que en tec4): tests con opciones equilibradas en
longitud, erratas de contenido, desbordes en móvil, docs al día. Lo que queda está en
`documentacion/PENDIENTES.md`.

Convenciones:
- Los tests de autocomprobación tienen las opciones equilibradas en longitud: al añadir preguntas, la correcta no debe ser la más larga.
- El libro es material de apoyo: no ampliar texto; sí figuras donde el contenido es visual.

## Cómo arrancar conmigo

Cuando vuelva, espera a que te diga la tarea. No audites el repo ni propongas cosas por tu cuenta. Solo:

1. Lee este kit.
2. Confirma "listo, todo cargado" y queda a la espera.
3. Yo te indico la tarea concreta.

Si la tarea no es de este repo (TyD 3º ESO), avisa para abrir un chat separado para el repo correspondiente.
