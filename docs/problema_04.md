# Problema 4: La Cinta Transportadora

**Asignatura:** Bases de Programación
**Unidad:** Algoritmos y Flujo de Control
**Archivo de solución esperado:** `problema_04.py`

---

## Contexto

En una línea de producción, una cinta transportadora traslada cajas que son inspeccionadas una por una. El estado de cada caja en el lote se registra en la siguiente lista:

```python
lote = ["OK", "OK", "VACIO", "OK", "DAÑADO", "OK", "VACIO"]
```

## Reglas de negocio

* **"OK"**: la caja está en buen estado y se empaca; se incrementa el contador de cajas empacadas.
* **"VACIO"**: la posición está vacía (no hay caja); se ignora y se continúa con la siguiente posición usando `continue`.
* **"DAÑADO"**: la caja está dañada; se imprime un mensaje de alerta y se detiene el procesamiento de todo el lote usando `break`.

## Requisitos

Escribe un programa en Python que:

1. Recorra la lista `lote` con un ciclo `for`.
2. Para cada estado "OK", incremente un contador de cajas empacadas.
3. Para cada estado "VACIO", use `continue` para saltar a la siguiente iteración sin contar nada.
4. Para el estado "DAÑADO", imprima un mensaje de alerta y use `break` para detener el procesamiento inmediatamente (ninguna caja posterior al "DAÑADO" debe procesarse).
5. Al finalizar (ya sea por `break` o por terminar de recorrer la lista), imprima el **total de cajas empacadas** hasta ese momento.

## Consideraciones

* El procesamiento debe detenerse en el primer "DAÑADO" que se encuentre; las cajas posteriores en la lista no deben evaluarse ni contarse.
* El programa debe funcionar para cualquier lista de estados, no solo para los valores de ejemplo.
* El mensaje de alerta debe ser claro y descriptivo (por ejemplo, indicando en qué posición del lote se detectó la caja dañada).

## Ejemplo

Para `lote = ["OK", "OK", "VACIO", "OK", "DAÑADO", "OK", "VACIO"]`:

```
Caja dañada detectada. Deteniendo procesamiento.
Total de cajas empacadas: 3
```

> Nota: las dos últimas posiciones ("OK", "VACIO") no se procesan porque el `break` ocurre al llegar a "DAÑADO" (posición 5).
