# DM Matrix System - Coordenadas de Escena Activa

## Objetivo

El DM debe usar la matriz del mapa como sistema principal para ubicar personajes, enemigos, trampas, objetos interactuables y zonas importantes.

Este sistema se aplica cuando la escena ya fue inicializada con el protocolo de `LLM-EscenaFichaEstructura.md`.

La referencia oficial usa coordenadas tipo:

* Letras en el eje vertical: A-U.
* Numeros en el eje horizontal: 01-25.
* Cada cuadro representa 2 metros.

Ejemplo de posición:

* Baltharax está en E12.
* Una trampa está en H08.
* Un cofre está en K04.
* Un enemigo está en C15.

---

# Reglas de Uso de Coordenadas

## Regla global de matriz estandar

Todos los mapas tacticos deben usar la misma matriz base:

* Eje vertical: A-U (21 filas).
* Eje horizontal: 01-25 (25 columnas).
* Escala fija: 1 cuadro = 2 metros.

Formato canonico de coordenada:

* Una letra + dos digitos.
* Ejemplos validos: A01, B14, F08, U25.
* Ejemplos invalidos: A1, A2, AA01, V01, A26.

Limite oficial del mapa estandar:

* Esquina superior izquierda: A01
* Esquina superior derecha: A25
* Esquina inferior izquierda: U01
* Esquina inferior derecha: U25

## Excepcion por escena (override permitido)

Si una escena necesita rebasar el limite oficial, se permite hacerlo solo si queda declarado de forma explicita en el archivo de escena activa.

Reglas de la excepcion:

1. Debe declararse el rango extendido de filas y/o columnas en la escena activa.
2. Debe mantenerse la misma escala: 1 cuadro = 2 metros.
3. Debe mantenerse el mismo formato canonico (letra + dos digitos).
4. Si la escena no declara excepcion, se aplica automaticamente la matriz estandar A-U y 01-25.

## 1. Toda entidad importante debe tener coordenada

Cuando el DM describa la escena activa, debe registrar la posición aproximada de:

* Jugadores
* Enemigos
* NPCs
* Trampas
* Puertas
* Cofres
* Altares
* Objetos mágicos
* Zonas peligrosas
* Cobertura
* Puntos de interés

Formato recomendado:

```md
## Posiciones Actuales

### Jugadores
- Baltharax: E12
- Tatanius: F10
- Mejek: J08
- Keco: oculto en H14

### Enemigos
- Goblin 1: C09
- Goblin 2: D11

### Objetos interactuables
- Puerta azul sellada: A12-A15
- Cofre antiguo: K05
- Altar roto: D08

### Trampas o peligros
- Trampa de presión: G10
- Zona de escombros difícil: H06-H09
```

Para consistencia tactica, preferir siempre dos digitos en columnas:

* E12 ya cumple el formato canonico por tener dos digitos.
* Para columnas de un digito usar cero a la izquierda: H08, K04, C09.

---

# Movimiento

Cada cuadro equivale a 2 metros.

Cuando un personaje se mueva, el DM debe indicar:

1. Coordenada inicial.
2. Coordenada final.
3. Distancia aproximada.
4. Si el movimiento provoca consecuencias.

Ejemplo:

```md
Baltharax se mueve de E12 a E15.
Distancia: 3 cuadros = 6 metros.
No provoca ataque de oportunidad.
```

---

# Acciones con distancia

Cuando un jugador quiera atacar, investigar, esconderse o interactuar, el DM debe revisar la posición en la matriz.

Ejemplo:

```md
Tatanius quiere disparar al goblin en C15.

Tatanius está en F10.
Goblin está en C15.
Distancia aproximada: 8 cuadros = 16 metros.

El objetivo está dentro del rango del arma.
Puede atacar normalmente.
```

---

# Trampas y objetos ocultos

El DM puede tener coordenadas secretas que no revela al jugador hasta que sean descubiertas.

Ejemplo privado para el DM:

```md
## Elementos Ocultos DM

- Trampa de lanza: H12
- Símbolo mágico oculto: B14
- Compartimento secreto: K03
```

Formato recomendado:

* H12, B14 y K03.

Cuando un jugador se acerque o investigue, el DM puede pedir tirada.

Ejemplo:

```md
Mejek se mueve a H12.

Hay una trampa oculta en esa coordenada.
Pedir tirada de Percepción o Investigación según la acción declarada.
```

---

# Formato recomendado para escena activa

Cada escena debe tener este bloque:

```md
# Escena Activa

## Lugar
[Nombre del área]

## Estado general
[Combate, exploración, tensión social, descanso, etc.]

## Escala
Cada cuadro = 2 metros.

## Matriz estandar
Filas A-U, columnas 01-25.

## Excepcion de limites (solo si aplica)
- Limite estandar aplicado: si/no
- Si no: [definir filas y columnas extendidas]

## Posiciones actuales

### Jugadores
- Nombre: coordenada

### Aliados / Mascotas
- Nombre: coordenada

### Enemigos visibles
- Nombre: coordenada

### Objetos interactuables
- Objeto: coordenada

### Peligros visibles
- Peligro: coordenada

### Elementos ocultos para DM
- Elemento oculto: coordenada

## Notas tácticas
- Cobertura:
- Terreno difícil:
- Puertas:
- Iluminación:
- Sonidos:
- Riesgos:
```

---

# Regla para el DM

El DM no debe saturar la narración con coordenadas todo el tiempo.

Debe usar coordenadas cuando ayuden a resolver:

* Movimiento
* Ataques
* Distancias
* Posición relativa
* Trampas
* Cobertura
* Persecuciones
* Efectos de área
* Exploración táctica

En la narración normal, puede describir de forma natural.

Ejemplo narrativo:

“Baltharax avanza entre los escombros hacia la puerta azul.”

Ejemplo táctico:

“Baltharax se mueve de E12 a C13, quedando a 2 cuadros de la puerta azul.”

## Checklist rapido al crear escena

1. Confirmar si usa matriz estandar (A-U, 01-25) o excepcion declarada.
2. Mantener escala fija de 2 metros por cuadro.
3. Registrar coordenadas de criaturas, objetos clave y peligros.
4. Separar coordenadas visibles para jugadores y coordenadas ocultas del DM.
