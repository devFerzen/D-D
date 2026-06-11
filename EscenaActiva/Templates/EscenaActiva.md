# EscenaActiva

## Identidad
- **Nombre de la escena:** 
- **Nombre oficial de campaña / capítulo / área:** 
- **Lugar / mapa:** 
- **Descripción breve:** 
- **Contexto narrativo breve:** 

---

## Control narrativo de escena (obligatorio)
Este bloque evita narrativa infinita y fuerza cierre de escena.

- **Propósito dramático de escena:** 
- **Pregunta dramática de escena:** 
- **Entrada clara de escena (disparador):** 
- **Avance de arco claro (qué debe avanzar sí o sí):** 
- **Salida clara de escena (condición de cierre):** 
  - **Tipo de cierre principal:** objetivo cumplido / reloj de presión / híbrido
  - **Condición concreta de cierre:** 
- **Límite de expansión lateral permitido:** bajo / medio / alto
- **Regla de retorno al hilo principal:** 
  - **Disparador de retorno:** 
  - **Tiempo máximo antes de reconducir:** 
- **Referencia de arco principal en ficha global:** 
  - `EscenaActiva/CampañaFichaEstructura.md` sección de arco principal

---

## Sistema de Coordenadas de la Escena
- **Escala fija:** 1 cuadro = 2 metros
- **Formato canónico de coordenada:** letra + dos dígitos (ejemplo: A01, H08, U25)
- **Límite estándar aplicado:** sí / no
- **Si no aplica límite estándar, definir override:**
  - **Filas habilitadas:** 
  - **Columnas habilitadas:** 
  - **Motivo narrativo o táctico del override:** 

Notas:
- Si no se declara override, usar matriz estándar (filas A-U y columnas 01-25).
- Mantener siempre el formato con dos dígitos en columnas de un solo número (01-09).

---

## Capa Visible
Elementos que los jugadores pueden percibir sin tirada al entrar o al observar normalmente.

### Lista de elementos visibles
- **Elemento:** 
  - **Tipo:** objeto / criatura / detalle del entorno / salida / pista visible
  - **Posición en escenario:** 
  - **Descripción visible:** 
  - **Interacción obvia:** 
  - **Notas opcionales:** luz / ruido / olor / temperatura / magia / fragilidad / cobertura

- **Elemento:** 
  - **Tipo:** 
  - **Posición en escenario:** 
  - **Descripción visible:** 
  - **Interacción obvia:** 
  - **Notas opcionales:** 

---

## Capa Oculta
Elementos que los jugadores no conocen de inicio.

### Lista de elementos ocultos
- **Elemento oculto:** 
  - **Tipo:** objeto / criatura / trampa / pista / ruta / mecanismo
  - **Posición en escenario:** 
  - **Cómo puede descubrirse:** percepción / investigación / interacción / magia / tiempo / herramienta
  - **Requiere herramienta o condición:** 
  - **Resistencia o reacción especial:** 
  - **Qué revela o activa:** 
  - **Notas opcionales:** susceptible a ruido / fuerte a magia / débil a fuego / etc.

- **Elemento oculto:** 
  - **Tipo:** 
  - **Posición en escenario:** 
  - **Cómo puede descubrirse:** 
  - **Requiere herramienta o condición:** 
  - **Resistencia o reacción especial:** 
  - **Qué revela o activa:** 
  - **Notas opcionales:** 

---

## NPC o Criaturas Presentes
Incluye visibles, ocultos, aliados, enemigos, animales, testigos, patrullas o emboscadas.

### Entidades presentes
- **Nombre:** 
  - **Tipo:** NPC / enemigo / monstruo / animal / aliado / testigo
  - **Visible al inicio:** sí / no
  - **Posición:** 
  - **Actitud inicial:** amistoso / neutral / hostil / alerta / asustado
  - **Objetivo actual:** 
  - **Qué sabe:** 
  - **Qué hace si no lo molestan:** 
  - **Qué hace si detecta al grupo:** 
  - **Qué hace si hay ruido / magia / combate:** 

- **Nombre:** 
  - **Tipo:** 
  - **Visible al inicio:** 
  - **Posición:** 
  - **Actitud inicial:** 
  - **Objetivo actual:** 
  - **Qué sabe:** 
  - **Qué hace si no lo molestan:** 
  - **Qué hace si detecta al grupo:** 
  - **Qué hace si hay ruido / magia / combate:** 

---

## Elementos interactivos y disparadores
Objetos que los jugadores podrían tocar, mover, romper, abrir, usar, inspeccionar o activar.

  - **Nombre:** Cofre de viaje
  - **Tipo:** objeto
  - **Posición:** pie de la cama
  - **Visible / oculto:** visible
  - **Qué parece:** un cofre común cerrado
  - **Cómo se interactúa o activa:** abrir, forzar, examinar
  - **Qué condición lo dispara:** abrir sin detectar la aguja
  - **Qué pasa si se activa:** dispara una aguja envenenada
  - **Qué tirada o mecánica puede entrar:** Investigación, Percepción, herramientas de ladrón
  - **Notas para improvisación:** si lo mueven bruscamente hace ruido

  - **Nombre:** Tabla suelta del suelo
  - **Tipo:** zona
  - **Posición:** junto a la ventana
  - **Visible / oculto:** oculto
  - **Qué parece:** suelo normal
  - **Cómo se interactúa o activa:** pisar encima
  - **Qué condición lo dispara:** peso suficiente sobre la tabla
  - **Qué pasa si se activa:** cruje fuerte y alerta al pasillo
  - **Qué tirada o mecánica puede entrar:** Percepción para detectarla
  - **Notas para improvisación:** también puede levantarse con cuidado

  - **Nombre:** Patrulla del pasillo
  - **Tipo:** evento
  - **Posición:** fuera de la habitación
  - **Visible / oculto:** oculto
  - **Qué parece:** no aplica
  - **Cómo se interactúa o activa:** ruido, demora o combate
  - **Qué condición lo dispara:** si el ruido sube o pasan 10 minutos
  - **Qué pasa si se activa:** entran dos guardias
  - **Qué tirada o mecánica puede entrar:** Sigilo, iniciativa
  - **Notas para improvisación:** si el grupo está callado, tardan más en llegar

---

## Riesgos
Elementos peligrosos o problemáticos de la escena que el DM debe conocer aunque los jugadores no.

- **Riesgo:** 
  - **Tipo:** trampa / patrulla / terreno / ruido / magia / clima / colapso / veneno / maldición
  - **Dónde aplica:** 
  - **Cómo se activa:** 
  - **Cómo se detecta:** 
  - **Consecuencia:** 
  - **Cómo escalarlo o suavizarlo:** 

- **Riesgo:** 
  - **Tipo:** 
  - **Dónde aplica:** 
  - **Cómo se activa:** 
  - **Cómo se detecta:** 
  - **Consecuencia:** 
  - **Cómo escalarlo o suavizarlo:** 

---

## Salidas
Vías por las que se entra, sale, huye o conecta la escena.

- **Salida:** 
  - **Tipo:** puerta / túnel / pasillo / escalera / ventana / pasadizo / ruta oculta
  - **Posición:** 
  - **Visible / oculta:** 
  - **Estado:** abierta / cerrada / bloqueada / sellada / vigilada
  - **Condición para usarla:** 
  - **A dónde lleva:** 
  - **Notas del DM:** 

- **Salida:** 
  - **Tipo:** 
  - **Posición:** 
  - **Visible / oculta:** 
  - **Estado:** 
  - **Condición para usarla:** 
  - **A dónde lleva:** 
  - **Notas del DM:** 

---

## FichaTactica
Resumen corto del entorno útil para improvisar y resolver acciones.

- **Tamaño del área:** 
- **Coberturas:** 
- **Alturas / desniveles:** 
- **Tipo de terreno:** normal / difícil / peligroso / estrecho / resbaladizo
- **Luz:** brillante / tenue / oscuridad
- **Sonidos relevantes:** 
- **Olores relevantes:** 
- **Temperatura / clima local:** 
- **Elementos reactivos a magia:** 
- **Elementos sensibles al ruido:** 
- **Puntos útiles para emboscada o defensa:** 

---

## Mecánicas más usables en esta escena
Lista breve de reglas o tiradas que el DM probablemente usará aquí.

- **Mecánica:** percepción
  - **Uso común en esta escena:** 
- **Mecánica:** investigación
  - **Uso común en esta escena:** 
- **Mecánica:** sigilo
  - **Uso común en esta escena:** 
- **Mecánica:** supervivencia
  - **Uso común en esta escena:** 
- **Mecánica:** persuasión / engaño / intimidación
  - **Uso común en esta escena:** 
- **Mecánica:** iniciativa / cobertura / terreno difícil / herramientas / magia
  - **Uso común en esta escena:** 

---

## Trazabilidad narrativa de la escena
Registro operativo para saber qué avanzó, qué quedó pendiente y cómo retomarlo.

### Piezas de historia con mayor avance en esta escena
- **Pieza de historia:** 
  - **Tipo:** canon principal / subtrama / personal de personaje
  - **Evidencia de avance en escena:** 
  - **Estado al cierre:** abierta / parcial / resuelta
  - **Referencia de continuidad:** `Sesiones/sesionActual.md` o archivo de sesión correspondiente

- **Pieza de historia:** 
  - **Tipo:** 
  - **Evidencia de avance en escena:** 
  - **Estado al cierre:** 
  - **Referencia de continuidad:** 

### Piezas de historia con menor avance o estancadas
- **Pieza de historia:** 
  - **Causa del bajo avance:** 
  - **Riesgo narrativo si se ignora:** 
  - **Acción sugerida para retomarla:** 
  - **Referencia de continuidad:** `Sesiones/sesionActual.md` o archivo de sesión correspondiente

- **Pieza de historia:** 
  - **Causa del bajo avance:** 
  - **Riesgo narrativo si se ignora:** 
  - **Acción sugerida para retomarla:** 
  - **Referencia de continuidad:** 

### Interacción de personajes con piezas narrativas
- **Mayor interacción:**
  - **Personaje:** 
  - **Pieza de historia:** 
  - **Impacto en escena:** 
  - **Referencia en personaje:** `Personajes/<Nombre>/notas-campaña.md`

- **Menor interacción (oportunidad de mejora):**
  - **Personaje:** 
  - **Pieza potencial relevante:** 
  - **Gancho sugerido para próxima escena:** 
  - **Referencia en personaje:** `Personajes/<Nombre>/notas-campaña.md`


## Notas breves para improvisación del DM
- **Detalles de ambiente que conviene recordar:** 
- **Detalles reactivos a magia:** 
- **Detalles reactivos a ruido:** 
- **Detalles reactivos a fuego, agua, oscuridad o movimiento:** 
- **Pistas que conectan con otra escena:** 