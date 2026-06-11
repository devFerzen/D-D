# Gobernanza de memoria y persistencia (DM)

## Objetivo

Definir donde se guarda cada tipo de informacion para evitar perdida de continuidad, duplicaciones y dependencia de memoria de chat.

Regla base: lo canónico de campaña vive en archivos del repositorio. La memoria de chat se usa solo para metadatos minimos operativos.

---

## Regla de precedencia de persistencia

1. Si impacta narrativa, estado de escena, estado de sesion o evolucion de personaje, se guarda en el repositorio.
2. Si es metadato breve para operacion del agente (recordatorio tecnico), puede ir en memoria minima.
3. Si hay duda, guardar en repositorio y no en memoria de chat.

---

## Mapa de destino obligatorio

- `EscenaActiva/`: estado operativo de la escena actual.
- `EscenaActiva/Templates/CampañaFichaEstructura.md`: estado macro de arcos, balance canon/desvio y control de continuidad.
- `Sesiones/sesionActual.md`: continuidad cronologica de lo ocurrido y punto de cierre/apertura.
- `Personajes/`: evolucion individual, capacidades, inventario, magia y notas persistentes por personaje.

---

## Que SI puede guardarse en memoria minima

Solo metadatos cortos del agente, por ejemplo:

- convenciones de estructura de carpetas,
- checklists operativos breves,
- recordatorios de enlaces entre documentos,
- decisiones de navegacion del repositorio.

Condiciones:

- maximo breve (1-5 lineas por nota),
- sin narrativa de campaña,
- sin estado jugable de escena,
- sin reemplazar datos que deban vivir en archivos del repo.
- si es una pregunta pendiente para el usuario, guardar solo resumen corto y estado (abierta/resuelta).

---

## Dudas bloqueantes: regla de consulta al usuario

Si el DM tiene una duda que bloquea una decision relevante, debe resolverla primero con el usuario.

Se considera duda bloqueante cuando falta informacion que cambia:

- continuidad narrativa,
- riesgo o consecuencia,
- estado de personajes o recursos,
- lectura correcta de objetivo o foco de escena.

Protocolo obligatorio:

1. Detener decision que depende del dato faltante.
2. Preguntar al usuario de forma directa y concreta.
3. Registrar la respuesta en archivo canonico del repositorio.
4. Marcar la pregunta como resuelta (si se habia guardado como metadato minimo).

---

## Que NO se guarda en memoria de chat

- resultados de escenas,
- cambios de recursos o consecuencias de personajes,
- avances de arcos o subarcos,
- posiciones tacticas, iniciativa, trampas, rutas o secretos,
- cualquier dato que otro DM o usuario deba poder auditar leyendo el repo.

---

## Regla de no duplicacion

Si el dato ya existe en un archivo canonico, no copiar texto largo en otra parte: dejar referencia al archivo origen.

---

## Protocolo rapido antes de cerrar turno

1. Verificar si hubo cambios de estado jugable o narrativo.
2. Persistir primero en `EscenaActiva`, `Sesiones` o `Personajes` segun corresponda.
3. Usar memoria minima solo si hace falta un metadato operativo corto.
4. Evitar guardar en memoria cualquier dato que deba sobrevivir por trazabilidad de campaña.
5. Si quedan preguntas bloqueantes abiertas, dejarlas en metadato minimo y resolverlas con el usuario antes de avanzar.
