# Protocolo operativo de arranque: EscenaActiva y CampanaFichaEstructura

## Objetivo

Antes de iniciar la narracion, el DM debe tener preparada la informacion base de la escena en archivos de `EscenaActiva` y una vista resumida de estado en `CampanaFichaEstructura`.

Este protocolo evita que el DM tenga que recorrer todo el repositorio en cada turno: define que consultar, en que orden y que dejar escrito antes de empezar.

---

## Regla principal

No se inicia narracion nueva si no existe una escena activa documentada y una ficha de campana actualizada para el momento actual.

---

## Fuentes obligatorias de informacion

1. `Sesiones/sesionActual.md` para continuidad narrativa y estado previo.
2. `Personajes/` para datos jugables y situacion individual de cada personaje.
3. `EscenaActiva/Templates/EscenaActiva.md` para crear el archivo de escena.
4. `EscenaActiva/Templates/CampanaFichaEstructura.md` para estado global.
5. `Mds/11-CoordenadasTacticas.md` si la escena amerita mapa tactico.
6. `Mds/04-GobernanzaMemoriaPersistencia.md` para decidir que va a archivos del repo y que puede quedar como metadato minimo.

---

## Flujo de arranque obligatorio (pre-narracion)

### Paso 1. Determinar continuidad y foco de escena

- Leer el punto de cierre de `sesionActual.md`.
- Definir: lugar, tension actual, objetivo inmediato y riesgo.
- Determinar si la escena requiere posicion tactica o se puede manejar narrativamente.

### Paso 2. Crear o actualizar archivo de EscenaActiva

- Basarse en `EscenaActiva/Templates/EscenaActiva.md`.
- Completar identidad, capa visible, capa oculta, entidades, riesgos, salidas y ficha tactica.
- Completar bloque de coordenadas y registrar posiciones de:
	- jugadores,
	- enemigos,
	- npc (si hay),
	- objetos interactuables,
	- trampas/peligros,
	- elementos ocultos para DM.

- Dejar previsual minima de la siguiente escena con:
	- titulo tentativo,
	- 1 a 3 detalles opcionales de conexion narrativa.

### Paso 3. Crear o actualizar CampanaFichaEstructura

- Basarse en `EscenaActiva/Templates/CampanaFichaEstructura.md`.
- Completar estado global del grupo, objetivo actual, presion y peligro.
- Cargar personajes en escena con informacion sintetica tomada de `Personajes/`.
- Para ubicar rapido que leer por personaje, usar `Personajes/README.md`.
- Registrar posicion en escena e iniciativa cuando aplique.

### Paso 4. Validar control narrativo antes de narrar

Antes de pasar a coordenadas o apertura de escena, dejar explicitados en `EscenaActiva`:

- proposito dramatico de escena,
- pregunta dramatica de escena,
- entrada clara de escena,
- avance de arco claro,
- salida clara de escena,
- limite de expansion lateral,
- regla de retorno al hilo principal.

Regla: si falta cualquiera de esos puntos, no inicia narracion.

### Paso 5. Confirmar sistema de coordenadas obligatorio

Toda escena se registra con coordenadas tacticas.

- Aplicar `11-CoordenadasTacticas.md` como formato base.
- Definir matriz activa (filas y columnas).
- Validar que entidades y objetos mapeados tengan coordenada.
- Si hay elementos ocultos, registrarlos solo en capa privada del DM.

### Paso 6. Preparar mapa para jugadores y capa privada del DM

- Mapa para jugadores: limpio, sin secretos marcados.
- Datos privados del DM: ubicacion real de trampas, items ocultos, rutas secretas y enemigos ocultos en el archivo de escena activa.

Regla: el mapa visible no debe revelar informacion oculta que los jugadores aun no descubren.

### Paso 7. Iniciar narracion

Solo despues de completar los pasos anteriores, el DM inicia la narracion de apertura de escena.

### Paso 8. Resolver dudas bloqueantes con el usuario

Si existe una duda que cambia decisiones relevantes de escena, el DM la consulta primero con el usuario y solo despues continua.

Aplicar la regla y protocolo definidos en `Mds/04-GobernanzaMemoriaPersistencia.md`.

---

## Regla de trazabilidad y no duplicacion

Para evitar ruido y mantenimiento pesado:

- `EscenaActiva` guarda estado operativo de la escena actual.
- `CampanaFichaEstructura` guarda el control macro de arcos y balance canon/desvio.
- `Sesiones/` guarda la continuidad cronologica de lo ocurrido.
- `Personajes/` guarda evolucion individual y notas persistentes.

Cuando un dato ya exista en otro archivo, no copiar texto largo: usar referencia al archivo origen.

Para cualquier duda entre guardar en memoria de chat o en archivos del repo, aplicar `Mds/04-GobernanzaMemoriaPersistencia.md`.

---

## Prompt de apoyo para imagen

Para generar mapa base de jugadores:

1. Copiar plantilla de `Help/TemplatesPrompts/Prompt-CreacionEscenarioImagen.md`.
2. Completar el bloque de salida para prompt en `EscenaActiva` con informacion solo visible para jugadores.
3. Ajustar descripcion de escena y layout tactico desde ese bloque.
4. Guardar variante de uso en `Help/PromptImagen/`.

Importante:
- El agente DM no ejecuta el prompt de imagen.
- El agente DM prepara el paquete de prompt para que el usuario lo use en otro chat de imagen.

El prompt final para jugadores debe mantener:

- cuadricula visible,
- coordenadas de borde,
- escala,
- sin marcadores de secretos.

Opcional:
- usar simbologia visible para NPC, objetos y peligros que los jugadores si pueden ver,
- incluir leyenda corta de esos simbolos visibles.

---

## Checklist rapido de arranque

1. Escena activa creada o actualizada.
2. CampanaFichaEstructura creada o actualizada.
3. Personajes en escena cargados desde `Personajes/`.
4. Coordenadas definidas y mapeo minimo completo en toda escena.
5. Separacion clara entre informacion visible de jugadores y datos ocultos del DM.
6. Control narrativo validado: entrada clara, avance de arco y salida clara.
7. Limite de expansion lateral y regla de retorno al foco principal definidos.
8. Dudas bloqueantes resueltas con el usuario (si existian).
9. Narracion iniciada solo despues del registro minimo.
