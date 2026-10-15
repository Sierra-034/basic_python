# Problema 5: El Mapa de la Sala de Cine

**Asignatura:** Bases de Programación
**Unidad:** Algoritmos y Flujo de Control
**Archivo de solución esperado:** `problema_05.py`

---

## Contexto

Se desea generar el mapa de asientos de una sala de cine para mostrarlo en pantalla antes de la venta de boletos. La sala está organizada en **filas** identificadas por letras y **asientos** identificados por números dentro de cada fila.

## Datos de la sala

* Filas: **'A', 'B', 'C'** (3 filas).
* Asientos por fila: **1 al 4** (4 asientos por fila).
* El identificador de cada asiento se forma concatenando la letra de la fila y el número de asiento (por ejemplo, "A1", "C4").

## Regla de negocio

* El asiento **"B3"** está reservado. En lugar de imprimir su identificador normal, debe mostrarse como **"[X]"**.
* Todos los demás asientos se muestran con su identificador normal (letra + número).

## Requisitos

Escribe un programa en Python que:

1. Utilice **ciclos `for` anidados**: un ciclo externo que recorra las filas y un ciclo interno que recorra los números de asiento.
2. Para cada asiento, determine si corresponde al asiento reservado ("B3"); si es así, imprima "[X]"; si no, imprima el identificador del asiento (letra + número).
3. Imprima los asientos de cada fila en una misma línea, separados por un espacio.
4. Al terminar una fila, pase a la siguiente línea antes de imprimir la fila siguiente.

## Consideraciones

* El formato de salida debe respetar exactamente el orden fila por fila, y dentro de cada fila, asiento por asiento en orden ascendente (1, 2, 3, 4).
* Los asientos deben separarse por un solo espacio, sin espacios adicionales al inicio o final de la línea.

## Salida esperada

```
A1 A2 A3 A4
B1 B2 [X] B4
C1 C2 C3 C4
```
