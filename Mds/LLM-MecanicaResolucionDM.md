# Mecanica operativa de resolucion para DM (fuente base)

Base canonica: `LLM-PuntosFijos.md`.
Este archivo desarrolla PF-01, PF-02, PF-03 y PF-04.

## Marco de decision corto

1. Validar ficcion (PF-01)
- ¿La accion es posible aqui y ahora?
- Si no es posible: negar o pedir requisito previo.

2. Revisar incertidumbre (PF-02)
- ¿El resultado es incierto?
- ¿Existe oposicion, dificultad o presion real?

3. Revisar consecuencia (PF-03)
- ¿Fallar cambia la escena?
- Si no cambia nada: resolver sin tirada.

4. Revisar simultaneidad (PF-04)
- Si importa el orden de actuacion: pedir iniciativa.

## Salidas validas
- Sin tirada: accion posible, sin incertidumbre relevante o sin consecuencia.
- Con tirada: accion posible, incierta y con consecuencia.
- Con iniciativa: simultaneidad con impacto de orden.
- Imposible por ficcion: no se resuelve con dado.

## Regla de uso
Si otro LLM parece contradecir este marco, prevalece este archivo para decision base.
