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
5. `Mds/LLM-CoordenadasDeEscena.md` si la escena amerita mapa tactico.

---

## Flujo de arranque obligatorio (pre-narracion)

### Paso 1. Determinar continuidad y foco de escena

- Leer el punto de cierre de `sesionActual.md`.
- Definir: lugar, tension actual, objetivo inmediato y riesgo.
- Determinar si la escena requiere posicion tactica o se puede manejar narrativamente.

### Paso 2. Crear o actualizar archivo de EscenaActiva

- Basarse en `EscenaActiva/Templates/EscenaActiva.md`.
- Completar identidad, capa visible, capa oculta, entidades, riesgos, salidas y ficha tactica.
- Si hay mapa, completar bloque de coordenadas y registrar posiciones de:
	- jugadores,
	- enemigos,
	- objetos interactuables,
	- trampas/peligros,
	- elementos ocultos para DM.

### Paso 3. Crear o actualizar CampanaFichaEstructura

- Basarse en `EscenaActiva/Templates/CampanaFichaEstructura.md`.
- Completar estado global del grupo, objetivo actual, presion y peligro.
- Cargar personajes en escena con informacion sintetica tomada de `Personajes/`.
- Registrar posicion en escena e iniciativa cuando aplique.

### Paso 4. Decidir si aplica sistema de coordenadas

Aplicar `LLM-CoordenadasDeEscena.md` cuando:

- importe distancia, alcance, cobertura o orden de movimiento,
- existan trampas, objetos ocultos o enemigos escondidos,
- haya persecucion, combate, infiltracion o exploracion tactica.

Si no aplica coordenada, dejarlo explicitado en la escena y resolver por ficcion.

### Paso 5. Preparar mapa para jugadores y capa privada del DM

- Mapa para jugadores: limpio, sin secretos marcados.
- Datos privados del DM: ubicacion real de trampas, items ocultos, rutas secretas y enemigos ocultos en el archivo de escena activa.

Regla: el mapa visible no debe revelar informacion oculta que los jugadores aun no descubren.

### Paso 6. Iniciar narracion

Solo despues de completar los pasos anteriores, el DM inicia la narracion de apertura de escena.

---

## Prompt de apoyo para imagen

Para generar mapa base de jugadores:

1. Copiar plantilla de `Help/TemplatesPrompts/Prompt-CreacionEscenarioImagen.md`.
2. Ajustar descripcion de escena.
3. Guardar variante de uso en `Help/PromptImagen/`.

El prompt final para jugadores debe mantener:

- cuadricula visible,
- coordenadas de borde,
- escala,
- sin marcadores de secretos.

---

## Checklist rapido de arranque

1. Escena activa creada o actualizada.
2. CampanaFichaEstructura creada o actualizada.
3. Personajes en escena cargados desde `Personajes/`.
4. Coordenadas definidas si la escena las necesita.
5. Separacion clara entre informacion visible de jugadores y datos ocultos del DM.
6. Narracion iniciada solo despues del registro minimo.
