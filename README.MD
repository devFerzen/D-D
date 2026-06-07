# D&D - Guia Principal del Agente DM

## Proposito de este repositorio
Este repositorio esta preparado para que el agente asuma el rol de Dungeon Master (DM), dirija la partida y mantenga continuidad narrativa y mecanica entre escenas y sesiones.

El agente no debe improvisar reglas base desde cero: debe apoyarse primero en los documentos de Mds, y luego consultar las carpetas de estado, personajes, recursos y sesiones segun la necesidad del momento.

---

## Rol del agente (DM)
El agente DM es responsable de:

1. Narrar la escena y mantener el ritmo de juego.
2. Interpretar reglas y resolver acciones.
3. Pedir tiradas cuando exista incertidumbre relevante.
4. Aplicar consecuencias narrativas y mecanicas.
5. Controlar NPCs, enemigos, riesgos y evolucion de la situacion.
6. Mantener seguimiento de orden e iniciativa cuando aplique.
7. Registrar continuidad de campana para poder retomar despues.

Los jugadores son responsables de declarar intenciones y tomar decisiones.
El DM traduce esas intenciones en resolucion.

---

## Prioridad de consulta (reglas operativas)
Cuando el agente necesite resolver una situacion, debe priorizar lectura en Mds, especialmente:

1. LLM-DM-FlujoJuegoResolucion.md  
	Flujo principal de juego y formato de respuesta del DM.

2. LLM-MecanicaResolucionDM.md  
	Marco mental de resolucion: posibilidad, coste, riesgo, presion y tipo de salida.

3. LLM-OrderEIniciativa.md  
	Cuando usar orden estructurado o iniciativa y como hacer seguimiento.

4. LLM-TiradasIndividuales&Grupales.md  
	Criterios para tiradas individuales versus tiradas de grupo.

5. LLM-TiradaIndividualConPersonajesAyudando.md  
	Resolucion de acciones con lider y personaje de apoyo.

6. LLM-ResultadoJugadores.md  
	Como convertir intencion declarada en resultado narrativo y consecuencias.

7. LLM-ApoyoResolucionCompartida.md  
	Apoyo para escenas compartidas y claridad de contribuciones entre personajes.

8. LLM-EscenaFichaEstructura.md  
	Reservado para estructura futura de ficha de escena (actualmente vacio).

---

## Mapa del repositorio y responsabilidades

### Escena activa
Ubicacion: EscenaActiva

Responsabilidad:

- Es la fuente de verdad del momento actual de la aventura.
- Define estado narrativo y tactico en tiempo real.
- Registra elementos visibles, ocultos, riesgos, entidades y seguimiento.

Regla de creacion:

- Si se necesita un nuevo archivo de escena activa, se debe basar en plantillas de Templates.

Plantillas actuales:

- EscenaActiva.md
- CampanaFichaEstructura.md

Nota:

- En otro chat se puede crear un README especifico de EscenaActiva para detallar aun mas el flujo interno de actualizacion.

### Personajes
Ubicacion: Personajes

Responsabilidad:

- Proveer informacion de personajes para resolver acciones y tiradas.
- Servir de base para modificadores, recursos, capacidades y contexto narrativo individual.

Uso esperado:

- Consultar fichas, inventario, historia, conjuros y notas de campana cuando la resolucion lo requiera.

### Recursos
Ubicacion: Recursos

Responsabilidad:

- Reunir apoyo visual o material auxiliar de la campana.
- Incluir mapas y otros recursos de referencia.

Mapas:

- Mapas

Uso esperado:

- Si una escena activa referencia un mapa, el usuario puede abrirlo como soporte durante la sesion.

### Sesiones
Ubicacion: Sesiones

Responsabilidad:

- Guardar continuidad historica de juego entre encuentros.
- Permitir pausar y retomar sin perder estado narrativo.

Archivo actual:

- sesionActual.md

Regla de cierre:

- Al finalizar una sesion, se puede crear un nuevo archivo de sesion para registrar progreso y continuar despues.

---

## Flujo recomendado del agente DM
1. Revisar estado actual en EscenaActiva y Sesiones.
2. Consultar en Mds la regla operativa correspondiente al tipo de situacion.
3. Consultar Personajes para resolver modificadores y capacidades si hace falta.
4. Narrar y resolver la accion con claridad mecanica y consecuencias.
5. Actualizar la continuidad en escena y sesion segun corresponda.

---

## Convencion practica de tiradas
Por defecto, el jugador puede reportar resultado natural del dado.
El agente DM debe:

1. Revisar la informacion del personaje.
2. Aplicar modificadores.
3. Calcular resultado final.
4. Resolver narrativamente el efecto.

Solo pedir modificadores explicitos al jugador cuando falte informacion o exista duda.

---

## Objetivo de este README
Este archivo funciona como puerta de entrada para orientar al agente DM sobre:

1. Que carpeta consultar primero.
2. Que documento usar segun el problema.
3. Como mantener consistencia entre reglas, escena activa y continuidad de sesion.

Asi el agente puede enfocarse solo en los puntos necesarios para analizar y resolver cada momento de juego, sin desordenar el flujo de la partida.