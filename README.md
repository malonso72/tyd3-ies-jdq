# TyD 3º ESO · IES Jiménez de Quesada

**Tecnología y Digitalización · 3º ESO · Curso 2025-26**
Profesor: Manuel Alonso Herrera · Santa Fe (Granada)

Sitio estático servido por Cloudflare Workers Static Assets en
[tyd3-ies-jdq.malonso72.workers.dev](https://tyd3-ies-jdq.malonso72.workers.dev).

## Estructura

```
tyd3-ies-jdq/
├── index.html                  Hub principal con las 6 unidades
├── unidades/                   6 unidades didácticas
│   └── NN-slug/
│       ├── index.html          Hub de la unidad
│       ├── teoria.html
│       ├── actividades.html
│       └── img/
├── herramientas/
├── proyectos/
├── _soluciones/                Privado, NO se despliega
├── img/
├── assets/{css,js,templates}/
├── documentacion/              Privado: PROGRAMACION, DECISIONES, PENDIENTES
└── scripts/                    Auditoría
```

## Despliegue

```bash
python3 -m http.server 8000          # test local
python3 scripts/comprobar_enlaces.py # validación pre-push
npx wrangler deploy                  # deploy
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
