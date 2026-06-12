# Condiciones y efectos de D&D 5e

Referencia operativa para el DM. Cada entrada define la condición y los datos mecánicos necesarios para resolver salvaciones.

Fuente base: D&D 5e SRD 5.1 (System Reference Document).

Para agregar una condición custom, replicar el bloque de plantilla al final del archivo.

---

## Plantilla de entrada

```
### [Nombre de la condición]
- **Tipo:** condición / efecto / veneno / maldición / otro
- **Stat de salvación:** CON / DEX / SAB / INT / FUE / CAR
- **CD base (SRD):** fija (indicar valor) / variable (depende de fuente)
- **Efecto al fallar:** 
- **Efecto al superar:** 
- **Duración:** 
- **Nueva salvación para terminar:** sí / no — (si sí, cuándo y con qué CD)
- **Referencia SRD:** SRD 5.1 / PHB p.XXX
- **Notas:** 
```

---

## Condiciones canónicas

### Envenenado
- **Tipo:** condición
- **Stat de salvación:** CON
- **CD base (SRD):** variable (depende de la fuente del veneno)
- **Efecto al fallar:** desventaja en tiradas de ataque y de habilidad
- **Efecto al superar:** sin efecto
- **Duración:** hasta que se cure o pase el tiempo indicado por la fuente
- **Nueva salvación para terminar:** sí — al final de cada turno, misma CD (venenos con duración progresiva)
- **Referencia SRD:** SRD 5.1 — Conditions: Poisoned
- **Notas:** algunos venenos también infligen daño por veneno en el momento; revisar fuente específica

---

### Asustado
- **Tipo:** condición
- **Stat de salvación:** SAB
- **CD base (SRD):** variable (depende del efecto o criatura que lo causa)
- **Efecto al fallar:** desventaja en tiradas de habilidad y de ataque mientras la fuente del miedo sea visible; no puede moverse voluntariamente hacia la fuente
- **Efecto al superar:** sin efecto
- **Duración:** según fuente (concentración del lanzador / duración fija)
- **Nueva salvación para terminar:** sí — al final de cada turno, misma CD (según fuente)
- **Referencia SRD:** SRD 5.1 — Conditions: Frightened
- **Notas:** si el personaje no puede ver a la fuente, puede repetir la salvación al final de su turno

---

### Paralizado
- **Tipo:** condición
- **Stat de salvación:** CON (o el declarado por la fuente)
- **CD base (SRD):** variable
- **Efecto al fallar:** incapacitado, no puede moverse ni hablar; ataques contra él tienen ventaja; golpes a menos de 1,5m son críticos automáticos
- **Efecto al superar:** sin efecto
- **Duración:** según fuente
- **Nueva salvación para terminar:** sí — al final de cada turno, misma CD
- **Referencia SRD:** SRD 5.1 — Conditions: Paralyzed
- **Notas:** una de las condiciones más severas; confirmar fuente antes de aplicar

---

### Incapacitado
- **Tipo:** condición
- **Stat de salvación:** no aplica (se aplica como consecuencia, no como salvación)
- **CD base (SRD):** —
- **Efecto al fallar:** no puede realizar acciones ni reacciones
- **Efecto al superar:** —
- **Duración:** según fuente
- **Nueva salvación para terminar:** no (condición derivada)
- **Referencia SRD:** SRD 5.1 — Conditions: Incapacitated
- **Notas:** es componente de otras condiciones (Paralizado, Petrificado, etc.)

---

### Derribado (Prone)
- **Tipo:** condición
- **Stat de salvación:** no aplica directamente (se genera como consecuencia de efecto)
- **CD base (SRD):** —
- **Efecto:** desventaja en ataques; ataques cuerpo a cuerpo contra él tienen ventaja, ataques a distancia tienen desventaja
- **Para levantarse:** cuesta la mitad del movimiento del turno
- **Referencia SRD:** SRD 5.1 — Conditions: Prone
- **Notas:** puede ser forzado por hechizos de área, trampas de derribo o ataques especiales

---

### Cegado
- **Tipo:** condición
- **Stat de salvación:** DEX (o el declarado por la fuente)
- **CD base (SRD):** variable
- **Efecto al fallar:** no puede ver; falla automáticamente tiradas que requieran vista; ataques realizados con desventaja; ataques recibidos con ventaja
- **Efecto al superar:** sin efecto
- **Duración:** según fuente
- **Nueva salvación para terminar:** según fuente
- **Referencia SRD:** SRD 5.1 — Conditions: Blinded
- **Notas:** —

---

### Aturdido (Stunned)
- **Tipo:** condición
- **Stat de salvación:** CON (o el declarado por la fuente)
- **CD base (SRD):** variable
- **Efecto al fallar:** incapacitado, no puede moverse, solo puede hablar con dificultad; ataques contra él tienen ventaja; falla salvaciones de FUE y DEX
- **Efecto al superar:** sin efecto
- **Duración:** hasta el final del siguiente turno del atacante (según fuente)
- **Nueva salvación para terminar:** no siempre — depende de la fuente
- **Referencia SRD:** SRD 5.1 — Conditions: Stunned
- **Notas:** muy limitante; confirmar con fuente si hay salvación repetida

---

## Venenos (entradas base)

### Veneno básico (frasco)
- **Tipo:** veneno
- **Stat de salvación:** CON
- **CD base (SRD):** 10
- **Efecto al fallar:** 1d4 daño por veneno
- **Efecto al superar:** sin efecto
- **Duración:** inmediato (sin duración)
- **Nueva salvación para terminar:** no
- **Referencia SRD:** SRD 5.1 — Adventuring Gear: Poison (Basic)
- **Notas:** puede aplicarse a arma o munición; efecto al primer golpe exitoso

---

### Veneno de serpiente gigante
- **Tipo:** veneno
- **Stat de salvación:** CON
- **CD base (SRD):** 11
- **Efecto al fallar:** 3d6 daño por veneno + condición Envenenado por 1 hora
- **Efecto al superar:** mitad de daño, sin condición
- **Duración:** 1 hora (condición Envenenado)
- **Nueva salvación para terminar:** no
- **Referencia SRD:** SRD 5.1 — Giant Poisonous Snake
- **Notas:** —
