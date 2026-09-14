# Pendientes · TyD 3º ESO

Lista de lo que queda por completar. Se actualiza con cada sprint.

## Hecho (a fecha de septiembre de 2026)

- [x] U4: cuadernillo de 64 ejercicios integrado en `actividades/`.
- [x] Etiquetas «Próximamente» retiradas del índice.
- [x] Repo en git y worker desplegado con auto-deploy (`git push`).
- [x] Enlaces de repaso a TyD 2.º en los hubs (U1, U2, U3, U4, U5, U6), comprobados contra el repo de 2.º.
- [x] Limpieza de septiembre de 2026: 108 preguntas de test reequilibradas en longitud (antes la correcta
  era la más larga en 87), erratas en U6 (App Inventor genera un APK, no «código Java»; giroscopio no es
  brújula; caso COMPAS descrito como lo documentó ProPublica; dictamen de copyright de 2023), desbordes
  en móvil (libro U3, arduino-blink), README y KIT al día.

## Pendiente

- [ ] Figuras en los libros donde el contenido es visual (U2-U6 no tienen ninguna): mecanismos y
  motor en U4 (palanca, polea, engranajes, tren compuesto, biela-manivela, 4 tiempos), circuitos
  serie/paralelo/mixto y CGMP en U5 (o enlazar a los interactivos que ya lo hacen), red doméstica en U3,
  diagrama de flujo en U6. Se puede reutilizar `figuras.py` de la auditoría de tec4.
- [ ] Revisar contenido con fecha: prohibición UE de coches de combustión en 2035 (libro U4; la UE lo está
  revisando).
- [ ] Criterios de evaluación LOMLOE concretos por unidad y bullets Saber/Hacer/Aplicar (de Manuel).

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

- [x] Repo en git y worker desplegado (`tyd3-ies-jdq.malonso72.workers.dev`), auto-deploy con `git push`.
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
