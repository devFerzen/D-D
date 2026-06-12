# Tiradas de salvación

Base canonica: `00-PuntosFijosCanonicos.md`.
Este archivo desarrolla PF-11 y referencia PF-02, PF-03 y PF-10.

---

## Flujo de desencadenante

Las tiradas de salvación siguen un flujo reactivo, opuesto al flujo de acción del jugador.

```
Enemigo / trampa / efecto actúa
  → DM declara: fuente, stat, CD y efecto (antes de resolver)
    → Jugador(es) tira(n)
      → DM narra consecuencia según resultado
```

Regla: si la fuente, el stat o la CD no están declarados en EscenaActiva antes de la escena, el DM debe declararlos ahora antes de continuar (PF-11).

---

## Qué stat usar

Referencia base: D&D 5e SRD.

| Tipo de amenaza                         | Stat de salvación |
|-----------------------------------------|-------------------|
| Veneno / enfermedad / resistencia física | CON               |
| Explosión / proyectil de área / trampa física | DEX           |
| Miedo / encantamiento / efectos mentales | SAB              |
| Ilusión / confusión / engaño mágico     | INT               |
| Dominación / encantamiento social       | CAR               |
| Empuje / agarre / fuerza bruta          | FUE               |

Si el tipo de amenaza no encaja claramente, usar el stat que la amenaza supera en el jugador (regla de narrativa: ¿qué parte del personaje está siendo atacada?).

---

## Cómo fijar la CD

La CD debe declararse en el bloque "Amenazas activas de salvación" de EscenaActiva antes de iniciar la escena.

Fuentes válidas de CD:
- **Enemigo lanzador**: 8 + bonificador de competencia + modificador de stat del lanzador.
- **Veneno / trampa**: CD fija definida en la entrada de `Referencias/Condiciones-D5e.md` o declarada por el DM con justificación.
- **Efecto de campaña persistente**: CD registrada en `Personajes/<Nombre>/notas-campaña.md`.

No se permite derivar la CD on-the-fly sin referencia documentada.

---

## Modificadores de salvación del jugador

Los modificadores de salvación de cada personaje están calculados en su ficha:
`Personajes/<Nombre>/ficha.md`

El resumen operativo vive en `EscenaActiva/CampañaFichaEstructura.md` (campo: "Salvaciones / ataque base relevante").

---

## Interpretación del resultado

Usar las mismas categorías de `22-InterpretacionConsecuencias.md`:

- **Éxito**: efecto negado o reducido según lo declarado en EscenaActiva.
- **Éxito parcial** (si aplica por diseño del efecto): consecuencia menor o daño reducido.
- **Fallo**: efecto completo según lo declarado. La escena cambia. Aplicar PF-03 y PF-10.

Un fallo de salvación no congela la partida: genera nueva situación jugable.

---

## Condiciones y efectos canónicos

Para condiciones de D&D 5e (Envenenado, Asustado, Paralizado, etc.) usar:
`Referencias/Condiciones-D5e.md`

Si una condición no está en ese archivo, el DM puede agregarla usando el template del mismo archivo antes de aplicarla en escena.

---

## Salvaciones de campaña vs salvaciones de escena

| Tipo                                      | Dónde vive                                      |
|-------------------------------------------|-------------------------------------------------|
| Amenaza activa en la escena actual        | EscenaActiva → bloque "Amenazas activas de salvación" |
| Condición persistente que carga un personaje | `Personajes/<Nombre>/notas-campaña.md`       |
| Maldición o efecto de arco narrativo largo | `EscenaActiva/CampañaFichaEstructura.md`       |

---

## Referencias
- Puntos canónicos: `00-PuntosFijosCanonicos.md` (PF-02, PF-03, PF-10, PF-11)
- Consecuencias post-tirada: `22-InterpretacionConsecuencias.md`
- Pre-arranque de escena: `03-PrearranqueEscenaObligatorio.md`
- Condiciones D&D 5e: `Referencias/Condiciones-D5e.md`
