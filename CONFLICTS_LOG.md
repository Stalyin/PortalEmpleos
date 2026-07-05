# Registro de Conflictos - TalentLink

## Conflicto 1

- Fecha/Hora: 2026-07-04 09:38 PM
- Archivos afectados:
  - css/styles.css
    index.html
- Integrantes involucrados:
  - Victor Pilachanga
  - Cristian Peña
- Descripción del conflicto:
  El integrante Cristian Peña agrego una oferta laboral sin previo aviso, se acepto las dos ofertas laborales y codifico el css con un diseño diferente.

## Conflicto 2

- Fecha/Hora: 2026-07-04 11:00
- Archivos afectados:
  - css/styles.css
  - index.html
- Integrantes involucrados:
  - Víctor Pilachanga - Integrante B
  - Brayan Moran - Integrante C
- Descripción del conflicto:
  Al fusionar la rama `feature/oferta-brayan-cv3` (Integrante C) hacia `dev`, Git marcó
  conflicto en `css/styles.css` porque ambos integrantes habían modificado el mismo
  bloque de estilos: Integrante B agregó `flex-direction: column` manteniendo el
  selector por ID (`#contenedor-destacados`), mientras que Integrante C renombró ese
  mismo selector a `.destacados-container` para unificar la nomenclatura del proyecto.
  Esto arrastró un segundo conflicto en `index.html`, ya que el `<div>` del panel de
  destacados debía usar `id="contenedor-destacados"` o `class="destacados-container"`,
  pero no ambos a la vez.
- Decisión tomada:
  Se combinaron ambos cambios: se conservó el selector de clase `.destacados-container`
  propuesto por Integrante C (por consistencia de nomenclatura) junto con el
  `flex-direction: column` propuesto por Integrante B (por el layout ya aprobado),
  actualizando el `<div>` en `index.html` a `class="destacados-container"`.

## Conflicto 3

- Fecha/Hora: 2026-07-04 22:00
- Archivos afectados:
  - index.html
  - css/styles.css
  - CONFLICTS_LOG.md
- Integrantes involucrados:
  - Equipo completo
- Descripción del conflicto:
  Durante la preparación de la rama release/v1.0 se detectó que la Oferta C no estaba ubicada después de la Oferta B y que el registro de conflictos no mantenía un orden secuencial claro.
  También se identificó que el diseño visual podía mejorar antes de pasar a producción.
- Decisión tomada:
  Se reorganizaron las ofertas laborales en orden A, B y C.
  Se edito el cv1 con el nombre del integrante correspondiente.
  Se ordenó el archivo CONFLICTS_LOG.md como Conflicto 1, Conflicto 2 y Conflicto 3.
  Además, se mejoró el estilo general del portal usando un diseño más limpio, responsive y profesional.
