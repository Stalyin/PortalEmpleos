# Registro de Conflictos - TalentLink

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
