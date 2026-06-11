# D&D - Guia Principal del Agente DM

## Proposito de este repositorio
Este repositorio esta preparado para que el agente asuma el rol de Dungeon Master (DM), dirija la partida y mantenga continuidad narrativa y mecanica entre escenas y sesiones.

El agente no debe improvisar reglas base desde cero: debe apoyarse primero en los documentos de Mds, y luego consultar las carpetas de estado, personajes, recursos y sesiones segun la necesidad del momento.

---

## Prioridad de consulta (reglas operativas)
Cuando el agente necesite resolver una situacion, usar este orden:

1. LLM-PuntosFijos.md
2. LLM-DM-FlujoJuegoResolucion.md
3. LLM-MecanicaResolucionDM.md
4. LLM-OrdenEIniciativa.md
5. LLM-CoordenadasDeEscena.md
6. LLM-TiradasIndividualesYGrupales.md
7. LLM-TiradaIndividualConPersonajesAyudando.md
8. LLM-ResultadoJugadores.md
9. LLM-MecanicaResolucionPvP.md
10. LLM-EscenaFichaEstructura.md

---

## Si buscas X, abre Y (atajo rapido)

- Base canonica de reglas cortas (PF): `LLM-PuntosFijos.md`.
- Flujo general del DM y formato de salida: `LLM-DM-FlujoJuegoResolucion.md`.
- Decision base de accion: `LLM-MecanicaResolucionDM.md`.
- Orden e iniciativa: `LLM-OrdenEIniciativa.md`.
- Coordenadas y mapa tactico: `LLM-CoordenadasDeEscena.md`.
- Individual vs grupal: `LLM-TiradasIndividualesYGrupales.md`.
- Lider y apoyo: `LLM-TiradaIndividualConPersonajesAyudando.md`.
- Resultado y consecuencias: `LLM-ResultadoJugadores.md`.
- Conflicto entre jugadores (PvP): `LLM-MecanicaResolucionPvP.md`.
- Pre-arranque de escena y ficha: `LLM-EscenaFichaEstructura.md`.

---

## Regla de precedencia entre LLM

Si hay conflicto entre redacciones:

1. Prevalecen los puntos fijos de `LLM-PuntosFijos.md`.
2. Luego prevalece `LLM-MecanicaResolucionDM.md` para decision base.
3. Luego prevalece el documento especializado del caso (PvP, apoyo, grupal, coordenadas).
4. `LLM-DM-FlujoJuegoResolucion.md` organiza el orden de uso y formato final.

---

## Flujo recomendado del agente DM
1. Revisar estado actual en EscenaActiva y Sesiones.
2. Aplicar `LLM-EscenaFichaEstructura.md` antes de narrar.
3. Resolver accion con `LLM-MecanicaResolucionDM.md` y derivados segun caso.
4. Consultar Personajes para modificadores y capacidades.
5. Narrar con formato PF-10.
6. Actualizar continuidad en escena y sesion.
