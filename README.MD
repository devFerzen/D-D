# D&D - Guia Principal del Agente DM

## Proposito de este repositorio
Este repositorio esta preparado para que el agente asuma el rol de Dungeon Master (DM), dirija la partida y mantenga continuidad narrativa y mecanica entre escenas y sesiones.

El agente no debe improvisar reglas base desde cero: debe apoyarse primero en los documentos de Mds, y luego consultar las carpetas de estado, personajes, recursos y sesiones segun la necesidad del momento.

---

## Prioridad de consulta (reglas operativas)
Cuando el agente necesite resolver una situacion, usar este orden:

**FUNDACIONALES (leer siempre primero):**
1. 00-PuntosFijosCanonicos.md
2. 01-MecanicaBaseResolucion.md
3. 02-FlujoDMOrquestacion.md
4. 03-PrearranqueEscenaObligatorio.md
5. 04-GobernanzaMemoriaPersistencia.md

**ESPECIALIZADAS (segun tipo de accion):**
- Orden y tactica: 10-OrdenTacticoIniciativa.md, 11-CoordenadasTacticas.md
- Tiradas y resolucion: 20-TiradasIndividualVsGrupal.md, 21-TiradasConApoyo.md, 22-InterpretacionConsecuencias.md
- Conflicto: 30-ResolucionPvP.md

---

## Si buscas X, abre Y (atajo rapido)

**Fundacionales:**
- Puntos fijos canonicos (PF-01...PF-10): `00-PuntosFijosCanonicos.md`.
- Decision base: es posible/incierto/consecuencia: `01-MecanicaBaseResolucion.md`.
- Como coordinar multiples LLM: `02-FlujoDMOrquestacion.md`.
- Pre-arranque obligatorio de escena: `03-PrearranqueEscenaObligatorio.md`.
- Gobernanza de memoria y persistencia: `04-GobernanzaMemoriaPersistencia.md`.

**Tactica y orden:**
- Orden, iniciativa y seguimiento: `10-OrdenTacticoIniciativa.md`.
- Coordenadas y mapa tactico: `11-CoordenadasTacticas.md`.

**Tiradas y resolucion:**
- Individual vs grupal: `20-TiradasIndividualVsGrupal.md`.
- Con apoyo (lider y ayudante): `21-TiradasConApoyo.md`.
- Interpretacion de resultados y consecuencias: `22-InterpretacionConsecuencias.md`.

**Especializado:**
- Conflicto entre jugadores (PvP): `30-ResolucionPvP.md`.

**Datos de personajes:**
- Estructura de `Personajes/` y que leer por archivo: `Personajes/README.md`.

---

## Regla de precedencia entre LLM

Si hay conflicto entre redacciones:

1. Prevalecen los puntos fijos de `00-PuntosFijosCanonicos.md`.
2. Luego prevalece `01-MecanicaBaseResolucion.md` para decision base.
3. Luego prevalece el documento especializado del caso (30-ResolucionPvP.md, 21-TiradasConApoyo.md, 20-TiradasIndividualVsGrupal.md, etc).
4. `02-FlujoDMOrquestacion.md` organiza el orden de uso y formato final.

---

## Flujo recomendado del agente DM
1. Revisar estado actual en EscenaActiva y Sesiones.
2. Aplicar `03-PrearranqueEscenaObligatorio.md` antes de narrar (PF-09).
3. Resolver accion con `01-MecanicaBaseResolucion.md` y especializada segun caso.
4. Consultar Personajes para modificadores y capacidades.
5. Narrar con formato PF-10 (ver `00-PuntosFijosCanonicos.md`).
6. Actualizar continuidad en escena y sesion.
