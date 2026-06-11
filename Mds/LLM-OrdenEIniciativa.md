# Escena activa: orden, iniciativa y seguimiento de personajes

## Propósito
Cuando una escena requiere saber **quién actúa primero**, **desde qué lugar actúa cada personaje** o **qué personaje sigue**, el DM debe pedir iniciativa o establecer un orden de actuación claro y **documentarlo en la carpeta `/EscenaActiva`** para consulta rápida durante la partida.

Esto sirve como apoyo operativo para no perder el hilo de la escena.

---

## Regla principal
Si la escena tiene simultaneidad, presión, riesgo, posiciones relevantes o acciones que pueden interferirse entre sí, el DM no debe improvisar el orden mentalmente durante demasiado tiempo: debe **formalizar el orden**.

La herramienta recomendada es:

- **tirada de iniciativa**, si el orden puede cambiar por reflejos, tensión o reacción;
- **orden declarado por ficción**, si el orden ya es obvio y no requiere aleatoriedad.

---

## Cuándo pedir iniciativa

Pide iniciativa si ocurre una o más de estas condiciones:

- varios personajes quieren actuar casi al mismo tiempo,
- importa quién llega primero,
- importa quién está más expuesto,
- hay riesgo inmediato,
- una acción puede interrumpir o impedir otra,
- el DM necesita estructura para recorrer la escena personaje por personaje.

### Ejemplos
- alguien intenta correr hacia una puerta mientras otro cubre la retirada;
- un enemigo puede reaccionar si oye algo;
- varios personajes exploran una zona pero una mala decisión puede detonar peligro;
- la escena aún no es combate pleno, pero sí necesita orden táctico.

---

## Cuándo no hace falta iniciativa

No hace falta pedir iniciativa si:

- el orden no cambia el resultado,
- las acciones pueden resolverse sin tensión temporal,
- todos actúan sin interferirse,
- la escena puede resolverse solo aclarando qué hace cada personaje.

En ese caso, el DM igual debe ir **uno por uno**, pero sin convertir la escena en un orden rígido innecesario.

---

## Qué debe pensar el DM
Antes de pedir iniciativa, el DM debe preguntarse:

1. ¿Necesito saber quién va primero?
2. ¿La posición de cada personaje importa?
3. ¿Voy a consultar a cada personaje de forma individual?
4. ¿Puedo perder el seguimiento de quién ya actuó?
5. ¿La escena mejoraría con una estructura visible?

Si la respuesta es sí a varias de estas preguntas, conviene pedir iniciativa y registrar el orden.

---

## Qué debe registrar el DM en `/EscenaActiva`
El DM debería dejar documentado, como mínimo:

- nombre del personaje,
- iniciativa u orden,
- nombre del mapa en escena activa que se encuentra en /Recursos/Mapas
- posición o lugar relevante (usar coordenada tipo E12 cuando aplique mapa, ver LLM-CoordenadasDeEscena.md),
- intención actual,
- si ya actuó o sigue pendiente,
- notas breves de estado.

Esto permite consultar rápidamente quién sigue sin reconstruir la escena desde memoria.

---

## Plantilla sugerida de registro
````markdown name=EscenaActiva/escena-activa.md
# Escena activa
- Nombre Mapa:

## Estado general
- Tipo de escena:
- Riesgo actual:
- ¿Hay iniciativa?: sí / no

## Orden de actuación
1. Nombre — iniciativa — posición — intención
2. Nombre — iniciativa — posición/coordenada — intención
3. Nombre — iniciativa — posición/coordenada — intención

## Seguimiento
- Ya actuaron:
- Pendientes:
- Cambio reciente en la escena:
- Próximo en actuar: