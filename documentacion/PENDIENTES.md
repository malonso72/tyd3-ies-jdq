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
- [x] Sprint del 16 de septiembre de 2026: símbolos electrónicos SVG en `identifica-componente` de U5
  (sustituyen a los emojis, que además desinformaban), 9 figuras en el libro de U4, 4 en el de U2 y 3 de
  red en el de U3, las 27 imágenes del cuadernillo de U4 extraídas a `/img/u04` en WebP (la página pasa
  de 1335 KB a 78 KB y las imágenes de 944 KB a 223 KB, con `alt` real y `loading=lazy`),
  `relacion-transmision` convertido en simulador con ruedas que giran y deslizadores, el veto europeo
  de 2035 matizado en el libro de U4, y la foto de fachada de 398 KB a 158 KB.

## Pendiente

- [ ] Figuras en los libros que aún no tienen: circuitos serie/paralelo/mixto y CGMP en U5 (los
  interactivos `tipos-circuitos`, `cgmp` y `abierto-cerrado-cortocircuito` ya suman 19 SVG entre los
  tres: probablemente salga más a cuenta enlazarlos que redibujar), y diagrama de flujo en U6. Las dos
  son de 3.ª evaluación.
- [ ] Interactivos que son test de texto y podrían llevar dibujo: `identifica-material`,
  `proceso-fabricacion` y `red-domestica`. En `malware`, `detecta-sesgo` y `elige-tecnologia` no hay
  símbolo normalizado que dibujar y el test de texto se sostiene tal cual.
- [ ] Calculadoras que ganarían con deslizador en vez de casilla: `calculadora-mixtos` y
  `tren-compuesto` (el patrón está en `relacion-transmision`).
- [ ] Los 6 interactivos de dibujo técnico están duplicados byte a byte con tec4: cualquier arreglo hay
  que hacerlo dos veces. Un `assets/interactivos-compartidos/` + script de copia lo resolvería.
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
