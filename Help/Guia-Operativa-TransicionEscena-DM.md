# Guia operativa: transicion de escena para el agente DM

## Objetivo
Tener un flujo corto y repetible para pasar de una escena terminada a una escena nueva sin perder continuidad y sin empezar narrativa antes de tiempo.

Esta guia complementa el protocolo obligatorio de prearranque y las plantillas de EscenaActiva.

Referencias principales:
- `Mds/03-PrearranqueEscenaObligatorio.md`
- `Mds/04-GobernanzaMemoriaPersistencia.md`
- `EscenaActiva/Templates/EscenaActiva.md`
- `EscenaActiva/Templates/CampañaFichaEstructura.md`
- `Sesiones/sesionActual.md`

---

## Regla de oro
Si una escena termino y se abrira otra, la narrativa de la nueva escena no inicia hasta que exista:
1. EscenaActiva nueva o actualizada para la nueva situacion.
2. CampañaFichaEstructura actualizada.
3. Control narrativo validado (entrada, avance de arco, salida, limites y retorno).
4. Coordenadas cargadas y mapeo tactico minimo completo.

---

## Flujo de transicion (fin de escena A -> inicio de escena B)

### Paso 0. Cerrar escena A (2-3 minutos)
En la escena que termina, dejar por escrito:
- Que se resolvio.
- Que quedo pendiente.
- Que consecuencias inmediatas deja para la siguiente escena.
- Que piezas tuvieron mayor avance y menor avance.
- Que personajes tuvieron mayor y menor interaccion narrativa.

Guardar referencias a:
- `Sesiones/sesionActual.md`
- `Personajes/<Nombre>/notas-campaña.md` (solo si aplica)

### Paso 1. Actualizar continuidad de sesion
En `Sesiones/sesionActual.md`, registrar:
- Punto de cierre exacto de la escena A.
- Estado del grupo al cierre (riesgo, recursos, posicion general).
- Gancho de apertura de la escena B.

### Paso 2. Crear o preparar escena B en EscenaActiva
Usar `EscenaActiva/Templates/EscenaActiva.md` y completar primero:
- Identidad.
- Control narrativo de escena (obligatorio).
- Capa visible y capa oculta.
- Entidades presentes.
- Riesgos y salidas.
- Previsual de siguiente escena (titulo tentativo y conexiones opcionales).
- Salida para prompt de imagen de jugadores (sin secretos).

Toda escena usa coordenadas: completar matriz y posiciones.

Mapeo minimo obligatorio:
- Jugadores.
- Enemigos.
- NPC (si hay).
- Objetos interactuables.
- Peligros o trampas.
- Elementos ocultos del DM.

### Paso 3. Actualizar ficha global de campaña
En `EscenaActiva/Templates/CampañaFichaEstructura.md`, reflejar:
- Arco principal activo y proximo hito.
- Subarcos activos.
- Balance canon/desvio esperado y observado.
- Resumen de avance narrativo de la sesion guardada.

### Paso 4. Validar control narrativo antes de abrir
No iniciar narrativa hasta verificar estos 8 puntos:
1. Proposito dramatico definido.
2. Pregunta dramatica definida.
3. Entrada clara definida.
4. Avance de arco claro definido.
5. Salida clara definida.
6. Limite de expansion lateral definido.
7. Regla de retorno al foco principal definida.
8. Coordenadas y mapeo tactico minimo completos.

### Paso 5. Resolver dudas bloqueantes con el usuario
Si hay dudas que cambian decisiones relevantes, consultarlas primero con el usuario y registrar respuesta canonica antes de narrar.

Referencia: `Mds/04-GobernanzaMemoriaPersistencia.md`.

### Paso 6. Abrir narrativa de escena B
Solo aqui iniciar la narracion de apertura.

### Paso 7. Preparar handoff de prompt de imagen para el usuario
Cuando la escena ya esta validada:
- Preparar el prompt final usando `Help/TemplatesPrompts/Prompt-CreacionEscenarioImagen.md`.
- Copiar los datos desde "Salida para prompt de imagen de jugadores" en `EscenaActiva`.
- Entregar el prompt al usuario para que lo ejecute en otro chat de imagen.

Regla:
- El agente DM no ejecuta el prompt de imagen, solo prepara el handoff.

---

## Mini plantilla express (llenado rapido)

### A. Control narrativo minimo (EscenaActiva)
- Proposito dramatico:
- Pregunta dramatica:
- Entrada clara:
- Avance de arco claro:
- Salida clara:
- Limite lateral:
- Regla de retorno:
- Titulo tentativo de siguiente escena:
- Conexiones opcionales a siguiente escena (1-3):

### A2. Coordenadas minimas (EscenaActiva)
- Matriz de escena (filas y columnas):
- Jugadores ubicados:
- Enemigos ubicados:
- NPC ubicados (si hay):
- Objetos interactuables ubicados:
- Peligros/trampas ubicados:

### A3. Salida para prompt de imagen (EscenaActiva)
- Descripcion de escena para imagen (solo visible):
- Puertas y salidas visibles:
- Coberturas visibles:
- Objetos interactuables visibles:
- Peligros visibles:
- Usar simbologia visible (si/no):
- Incluir leyenda visible (si/no):

### B. Trazabilidad minima (EscenaActiva)
- Mayor avance (1-2 piezas):
- Menor avance (1-2 piezas):
- Mayor interaccion de personaje (1):
- Menor interaccion de personaje (1):

### C. Continuidad minima (CampañaFichaEstructura)
- Arco principal activo:
- Proximo hito:
- Balance canon/desvio:
- Semilla para retomar despues:

---

## Reglas de no duplicacion
- EscenaActiva: estado operativo de la escena actual.
- CampañaFichaEstructura: estado macro de arcos y balance de campaña.
- Sesiones: continuidad cronologica.
- Personajes: evolucion individual.

Si un dato ya existe en otro archivo, no copiar texto largo: solo referenciar archivo y seccion.

La memoria de chat solo se usa para metadatos minimos; nunca reemplaza persistencia canonica del repositorio.

---

## Criterio de calidad rapido (si/no)
- La escena nueva tiene inicio claro, avance claro y salida clara.
- El foco principal de campaña sigue visible.
- El desvio lateral esta limitado y controlado.
- Hay al menos una semilla clara para continuidad futura.
- La escena ya tiene coordenadas y posiciones tacticas mapeadas.
- La salida para prompt de imagen esta limpia de secretos DM.
- Se puede narrar sin releer todo el repositorio.

Si cualquier punto es "no", ajustar antes de iniciar narrativa.
