# TyD 3º ESO · IES Jiménez de Quesada

**Tecnología y Digitalización · 3º ESO · Curso 2026-27**
Profesor: Manuel Alonso Herrera · Santa Fe (Granada)

Sitio estático servido por Cloudflare Workers Static Assets en
[tyd3-ies-jdq.malonso72.workers.dev](https://tyd3-ies-jdq.malonso72.workers.dev).

## Estructura

```
tyd3-ies-jdq/
├── index.html                  Hub principal con las 6 unidades
├── unidades/
│   └── NN-slug/
│       ├── index.html          Hub de la unidad (Saber/Hacer/Aplicar + recursos)
│       ├── libro-digital.html  Teoría (teoria.html redirige aquí)
│       ├── interactivos/       Simuladores y microactividades
│       ├── actividades/        Ejercicios resueltos (actividades.html redirige aquí)
│       ├── autocomprobacion/   Test de 18 preguntas con corrección
│       └── proyecto/           Proyecto de la unidad con rúbrica
├── _soluciones/                Privado, NO se despliega
├── img/
├── assets/{css,js,templates}/
├── documentacion/              PROGRAMACION, DECISIONES, PENDIENTES (no se despliega)
└── scripts/                    Verificación (HTML, enlaces) y hook de pre-push
```

## Despliegue

`git push` a `main` despliega automáticamente en Cloudflare (integración con GitHub).
El hook de pre-push ejecuta antes los verificadores de HTML y enlaces y bloquea el push si algo falla.

```bash
python3 -m http.server 8000          # prueba local
python3 scripts/verificar_html.py    # HTML bien formado
python3 scripts/verificar_enlaces.py # enlaces y anclas
git push                             # despliega
```

## Versionado

SemVer. Versión actual visible en pie del index.

## Convenciones

- HTML + CSS + JS vanilla. Sin frameworks.
- Tipografía: Barlow + Barlow Condensed + JetBrains Mono.
- Paleta: burdeos (`--principal #8C2A3D`) con acento azul (`#1B4F8A`).
- Accesibilidad: skip-link, focus-visible, alt en imágenes, contraste AA.

## Enlaces cruzados

Las unidades U1, U4, U5 y U6 enlazan a su unidad equivalente de **TyD 2º ESO**
(`tyd2-ies-jdq.malonso72.workers.dev`) como repaso previo, según §6.3 del brief.

Modelo de referencia: `teci2-ies-jdq` (TECI II) y `tyd2-ies-jdq` (TyD 2º ESO).
