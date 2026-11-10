# Copa Interna PILE 2026

Sitio web oficial de la **Copa Interna PILE 2026**, campeonato interno de fútbol indoor. Permite consultar los equipos participantes, el calendario de partidos, los resultados, la tabla de posiciones y el desarrollo de la fase eliminatoria.

🌐 **Página oficial:** https://jorge2320023.github.io/copa-interna-pile/

## Sobre el campeonato

La competición cuenta con nueve equipos y se desarrolla en dos etapas:

- **Fase regular:** nueve fechas, cuatro partidos y un equipo libre por jornada. Cada equipo disputa ocho encuentros.
- **Fase eliminatoria:** playoffs, semifinales, partido por el tercer puesto y gran final.

## Funcionalidades

### Fase regular

- Calendario completo de las nueve fechas.
- Registro de resultados de cada encuentro.
- Actualización automática de la tabla de posiciones.
- Cálculo de partidos jugados (PJ), goles a favor (GF), goles en contra (GC), diferencia de gol (DG) y puntos (PTS).
- Identificación automática de los próximos encuentros y del equipo que descansa.
- Resolución de empates mediante los criterios establecidos.

**Criterios de desempate:**

1. Puntos (PTS).
2. Diferencia de gol (DG).
3. Goles a favor (GF).
4. Enfrentamiento directo.
5. Fair Play.
6. Sorteo.

Cuando los criterios automáticos no son suficientes, la clasificación queda pendiente de resolución manual.

### Fase eliminatoria

**Playoffs**

Los cruces se generan a partir de la clasificación final:

- PO1: segundo puesto vs. séptimo puesto.
- PO2: tercer puesto vs. sexto puesto.
- PO3: cuarto puesto vs. quinto puesto.

El primer lugar de la fase regular clasifica directamente a semifinales.

**Semifinales**

Los cuatro clasificados se determinan automáticamente, pero los enfrentamientos se asignan manualmente mediante sorteo.

**Partidos finales**

Los participantes del partido por el tercer puesto y de la gran final se identifican automáticamente a partir de los resultados de las semifinales.

El sistema también reconoce al campeón, subcampeón, tercer y cuarto puesto.

Los marcadores pueden incluir los resultados de penales cuando un encuentro se define por esa vía.

## Actualización y mantenimiento

El proyecto utiliza HTML, CSS y JavaScript. La administración y edición de los archivos se realiza mediante **Visual Studio Code (VS Code)**, conectado al repositorio de GitHub.

Las principales secciones que se deben modificar son:

| Variable | Función |
|---|---|
| `resultados` | Registrar los resultados de la fase regular. |
| `fixtureRegular` | Consultar o modificar el calendario y los horarios de la fase regular. |
| `desempateManual` | Introducir el orden definitivo cuando un empate requiere Fair Play o sorteo. |
| `playoffResultados` | Registrar los resultados de los tres partidos de playoffs. |
| `semifinales` | Asignar los equipos después del sorteo e introducir los resultados. |
| `tercerPuesto` | Registrar el resultado del partido por el tercer puesto. |
| `granFinal` | Registrar el resultado de la gran final. |
| `programacionEliminatoria` | Establecer los horarios de los partidos eliminatorios. |
| `playoffOficiales` | Confirmar y conservar los cruces definitivos de playoffs. |

### Procedimiento para actualizar la página

1. Abrir el proyecto en Visual Studio Code.
2. Localizar el archivo `index.html` y modificar la sección correspondiente según la etapa de la competición.
3. Guardar los cambios y comprobar que el código mantenga su estructura.
4. Abrir el apartado **Source Control** de VS Code para revisar los archivos modificados.
5. Escribir un mensaje descriptivo para el commit, por ejemplo: `Actualizar resultados de la fecha 5`.
6. Realizar el commit y sincronizar los cambios con GitHub mediante **Push** o **Sync Changes**.
7. GitHub Pages publicará la versión actualizada del sitio.

**Importante:** los resultados y las configuraciones se administran directamente desde el código. No se utiliza almacenamiento local (`LocalStorage`) para conservar los cruces oficiales, por lo que los visitantes consultan la misma información publicada.

## Tecnologías utilizadas

- HTML5
- CSS3
- JavaScript
- Visual Studio Code
- Git y GitHub
- GitHub Pages

## Repositorio

El proyecto se mantiene mediante Visual Studio Code y GitHub. Su publicación se realiza utilizando GitHub Pages.

**Copa Interna PILE 2026 — Calendario, resultados y seguimiento de la competición.**
