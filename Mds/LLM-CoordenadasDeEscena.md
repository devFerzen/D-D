# DM Matrix System - Coordenadas de Escena Activa

## Objetivo

El DM debe usar la matriz del mapa como sistema principal para ubicar personajes, enemigos, trampas, objetos interactuables y zonas importantes.

La escena usa coordenadas tipo:

* Letras en el eje vertical: A, B, C, D, E...
* Números en el eje horizontal: 1, 2, 3, 4, 5...
* Cada cuadro representa 2 metros.

Ejemplo de posición:

* Baltharax está en E12.
* Una trampa está en H8.
* Un cofre está en K4.
* Un enemigo está en C15.

---

# Reglas de Uso de Coordenadas

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
- Mejek: J8
- Keaz: oculto en H14

### Enemigos
- Goblin 1: C9
- Goblin 2: D11

### Objetos interactuables
- Puerta azul sellada: A12-A15
- Cofre antiguo: K5
- Altar roto: D8

### Trampas o peligros
- Trampa de presión: G10
- Zona de escombros difícil: H6-H9
```

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
- Compartimento secreto: K3
```

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
