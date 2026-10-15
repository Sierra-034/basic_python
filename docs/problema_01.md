# Problema 1: El Clasificador de Tarifas

**Asignatura:** Bases de Programación
**Unidad:** Algoritmos y Flujo de Control
**Archivo de solución esperado:** `problema_01.py`

---

## Contexto

Un parque de diversiones cobra la entrada según la edad del visitante y si cuenta con credencial escolar.

## Reglas de negocio

* Menores de 5 años: **Gratis ($0)**.
* Estudiantes (de 5 a 17 años):
  * **$50** si presentan credencial escolar.
  * **$80** si NO presentan credencial escolar.
* Adultos (de 18 a 60 años): **$120**.
* Adultos mayores (más de 60 años): **$40**.

## Requisitos

Escribe un programa en Python que:

1. Defina la variable `edad` (entero) con la edad del visitante.
2. Defina la variable `tiene_credencial` (booleano) que indique si el visitante presenta credencial escolar.
3. Calcule la tarifa correspondiente según las reglas de negocio anteriores.
4. Imprima el precio final con un mensaje claro y descriptivo (por ejemplo, indicando la categoría del visitante y el costo del boleto).

## Consideraciones

* Los límites de edad son inclusivos según lo descrito: 5 a 17 años corresponde a estudiantes, 18 a 60 años corresponde a adultos, y más de 60 años corresponde a adultos mayores.
* `tiene_credencial` solo debe afectar el cálculo cuando la edad corresponde al rango de estudiante.

## Ejemplos

| `edad` | `tiene_credencial` | Tarifa esperada |
|---|---|---|
| 3 | `False` | $0 |
| 10 | `True` | $50 |
| 16 | `False` | $80 |
| 35 | `False` | $120 |
| 70 | `False` | $40 |
