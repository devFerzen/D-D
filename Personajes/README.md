# Personajes - Estructura y guia rapida para DM

## Proposito

Esta carpeta centraliza la informacion jugable y narrativa de cada personaje.
Usala para cargar datos en escena activa y resolver acciones segun capacidades reales del grupo.

---

## Estructura esperada

Cada personaje se organiza con dos niveles:

1. Un archivo indice en raiz: `Personajes/<Nombre>.md`.
2. Una subcarpeta con detalle: `Personajes/<Nombre>/`.

Ejemplo:

- `Personajes/Mejek.md`
- `Personajes/Mejek/ficha.md`
- `Personajes/Mejek/inventario.md`
- `Personajes/Mejek/historia.md`
- `Personajes/Mejek/notas-campaña.md`
- `Personajes/Mejek/conjuros.md` (solo si aplica magia)

---

## Que contiene cada archivo

- `ficha.md`: datos base, combate, habilidades, rasgos, dotes y estructura de magia.
- `inventario.md`: armas, objetos y equipo fisico.
- `conjuros.md`: lista de magia preparada, espacios y notas de uso.
- `historia.md`: trasfondo y elementos narrativos del personaje.
- `notas-campaña.md`: recordatorios persistentes, ajustes de mesa y motor tactico personal.

---

## Flujo rapido para escena activa

Si necesitas cargar un personaje en `EscenaActiva`, usar este orden:

1. Abrir `Personajes/<Nombre>.md` para ver el mapa de archivos del personaje.
2. Leer `ficha.md` para modificadores, recursos y capacidades de accion.
3. Leer `inventario.md` si hay uso de equipo, objetos o armas.
4. Leer `conjuros.md` solo si el personaje usa magia.
5. Revisar `notas-campaña.md` para excepciones, recordatorios y estado persistente.
6. Consultar `historia.md` cuando la decision dependa de tono, motivacion o trasfondo.

---

## Regla de consistencia

- Si un personaje no usa magia, no se exige `conjuros.md`.
- Evitar duplicar informacion larga entre archivos: mantener el dato en su origen y referenciarlo.
