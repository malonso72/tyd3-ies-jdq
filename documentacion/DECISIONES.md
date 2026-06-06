# Decisiones de diseño · TyD 3º ESO

Bitácora de decisiones técnicas y editoriales del proyecto.
Formato: `YYYY-MM-DD · Decisión` con justificación.

## 2026-05-10 · Bootstrap del sitio (v1.0.0)

- **Modelo de referencia:** `teci2-ies-jdq` y `tyd2-ies-jdq`. Misma estructura
  modular, misma tipografía, misma filosofía vanilla.
- **Paleta burdeos** (`--principal #8C2A3D`). Justificación: progresión de
  saturación creciente con el curso (1º verde-cian → 2º naranja → 3º burdeos
  → 4º morado), todos diferenciables del azul TECI a primer vistazo.
- **Estructura por unidades didácticas integradas** (no por bloques temáticos).
  Cada unidad tiene `index.html` + `teoria.html` + `actividades.html` (+ `reto.html`
  opcional). En 3º ESO no hay U0 — el dibujo técnico ya es una unidad
  completa (U1) con perspectivas y normalización avanzada.
- **Slug numerado de 2 dígitos** (`01-...` a `06-...`) para que el orden
  alfabético coincida con el orden didáctico.
- **Enlaces cruzados a TyD 2º ESO** (§6.3 del brief): U1, U4, U5 y U6 llevan
  un callout visible enlazando a la unidad equivalente de 2º ESO como
  *"Repaso previo"*. URL absoluta al subdominio Cloudflare hermano para que
  funcione aunque se navegue offline desde una copia.
- **CSS modular** en cuatro archivos (`common`, `hub`, `unidad`, `proyecto`),
  paleta en `:root` de `common.css` para poder cambiarla en un solo sitio.
- **Solucionarios privados** en `_soluciones/`, excluidos del despliegue
  vía `.assetsignore`.

## Convenciones

- Slug de unidad: `NN-kebab-case` con dos dígitos (`01-`, `02-`, ...).
- Commits: español, verbo en imperativo, versión al final entre corchetes.
- Sin frameworks. Sin CDNs salvo Google Fonts y MathJax.
