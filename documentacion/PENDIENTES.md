# Pendientes · TyD 3º ESO

Lista de lo que queda por completar. Se actualiza con cada sprint.

## Bloqueante para v1.1.0 (Fase H del brief)

- [ ] **U4 Mecanismos y motores**: integrar `cuadernillo_ejercicios_3eso_v6.html`
  (64 ejercicios) en `unidades/04-mecanismos-motores/actividades.html`.
  Manuel debe indicar la ruta local del archivo. Aplicar paleta burdeos al
  CSS interno si fuera necesario, ajustar rutas a `assets/css/` y `assets/js/`
  del nuevo entorno. Verificar MathJax, vídeos y autocorrección.
- [ ] Si el cuadernillo trae teoría embebida, extraer a
  `unidades/04-mecanismos-motores/teoria.html`.
- [ ] Quitar el `<span class="pending-badge">Próximamente</span>` de la
  tarjeta U4 en el `index.html` cuando su material esté integrado.

## Pendientes de Manuel (no bloqueantes)

- [ ] **Criterios de evaluación LOMLOE concretos** por unidad. Rellenar el
  `<details class="criterios">` de cada hub.
- [ ] **Bullets de "saber/hacer/evaluar"**: los actuales son una primera
  aproximación al currículo LOMLOE Andalucía. Revisar y ajustar a la
  programación oficial del departamento.
- [ ] **Duración estimada de las unidades**: rangos orientativos. Validar
  con la programación didáctica del departamento.
- [ ] **Proyectos integradores**: definir y crear desde
  `assets/templates/PLANTILLA_proyecto.html`.
- [ ] **Herramientas**: añadir simuladores (mecanismos, circuitos), glosario.

## Infraestructura

- [ ] **`git init`**: el sistema en el que se generó este repo no tenía
  git instalado. Manuel debe ejecutar al recibirlo:
  ```bash
  cd tyd3-ies-jdq && git init -b main && git add . && \
  git commit -m "Bootstrap del sitio TyD 3º ESO [v1.0.0]"
  ```
- [ ] **Configuración del worker Cloudflare**: crear el subdominio
  `tyd3-ies-jdq.malonso72.workers.dev`. Probar primer deploy con
  `npx wrangler deploy`.
- [ ] **Google Search Console**: añadir verificación si se quiere indexar.

## Enlaces cruzados (§6.3 del brief)

Los siguientes hubs llevan un callout "Repaso previo" enlazando a TyD 2º ESO:

- U1 Dibujo técnico → `tyd2-ies-jdq.../unidades/00-dibujo-tecnico/`
- U4 Mecanismos y motores → `tyd2-ies-jdq.../unidades/04-maquinas-simples/`
- U5 Circuitos y robótica → `tyd2-ies-jdq.../unidades/05-electricidad/`
- U6 Programación e IA → `tyd2-ies-jdq.../unidades/07-programacion/`

> Los enlaces son URLs absolutas al subdominio Cloudflare hermano. Cuando el
> sitio TyD2 esté desplegado, los enlaces serán navegables. Mientras tanto,
> en local apuntan a un dominio que no existe (intencionalmente).
