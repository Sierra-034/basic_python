# Problema 2: El Radar de la Avenida

**Asignatura:** Bases de Programación
**Unidad:** Algoritmos y Flujo de Control
**Archivo de solución esperado:** `problema_02.py`

---

## Contexto

Un radar de tráfico sobre una avenida con límite de velocidad de **80 km/h** registró la velocidad de los siguientes 8 vehículos durante un intervalo de tiempo:

```python
velocidades = [75, 92, 80, 110, 68, 85, 99, 70]
```

## Requisitos

Escribe un programa en Python que, usando un ciclo `for` para recorrer la lista `velocidades`, calcule e imprima:

1. El **total de vehículos** que superaron el límite de velocidad.
2. La **velocidad más alta** registrada entre los infractores.
3. El **monto total recaudado en multas**, considerando que cada infracción cuesta **$500**.

## Consideraciones

* Un vehículo se considera infractor únicamente si su velocidad es **estrictamente mayor** a 80 km/h (es decir, viajar exactamente a 80 km/h no constituye infracción).
* El programa debe funcionar para cualquier lista de velocidades, no solo para los valores de ejemplo.
* Los resultados deben imprimirse con mensajes claros y descriptivos.

## Ejemplo

Para la lista `velocidades = [75, 92, 80, 110, 68, 85, 99, 70]`:

| Resultado | Valor |
|---|---|
| Vehículos infractores | 4 |
| Velocidad más alta (infractores) | 110 |
| Multas recaudadas | $2000 |
