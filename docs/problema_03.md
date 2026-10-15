# Problema 3: El Cajero Automático

**Asignatura:** Bases de Programación
**Unidad:** Algoritmos y Flujo de Control
**Archivo de solución esperado:** `problema_03.py`

---

## Contexto

Se requiere simular el acceso a un cajero automático, el cual solicita un NIP (número de identificación personal) y permite un número limitado de intentos antes de bloquear la tarjeta por seguridad.

## Reglas de negocio

* El NIP correcto es: **"4321"**.
* El usuario dispone de un máximo de **3 intentos**.
* Si el NIP ingresado es correcto:
  * Se imprime **"Acceso concedido"**.
  * El programa termina inmediatamente (sin seguir solicitando NIP).
* Si el NIP ingresado es incorrecto:
  * Se descuenta un intento.
  * Se muestra un mensaje indicando **cuántos intentos le quedan** al usuario.
* Si el usuario agota los 3 intentos sin ingresar el NIP correcto:
  * Se imprime **"Tarjeta bloqueada por seguridad"**.

## Requisitos

Escribe un programa en Python que:

1. Utilice un ciclo `while` para controlar el número de intentos disponibles (iniciando en 3).
2. En cada iteración, solicite al usuario el NIP mediante `input()`.
3. Compare el NIP ingresado contra el valor correcto ("4321").
4. Aplique la lógica de acceso concedido / intento fallido / bloqueo descrita en las reglas de negocio.

## Consideraciones

* El ciclo debe detenerse tan pronto se conceda el acceso (no debe seguir pidiendo el NIP después de un acierto).
* El ciclo debe detenerse también al agotarse los 3 intentos, mostrando el mensaje de bloqueo.
* Los mensajes de intentos restantes deben ser claros (por ejemplo, indicar el número exacto de intentos que quedan tras cada fallo).

## Ejemplo de ejecución

```
Ingresa tu NIP: 1111
NIP incorrecto. Te quedan 2 intentos.
Ingresa tu NIP: 2222
NIP incorrecto. Te quedan 1 intentos.
Ingresa tu NIP: 4321
Acceso concedido
```

```
Ingresa tu NIP: 1111
NIP incorrecto. Te quedan 2 intentos.
Ingresa tu NIP: 2222
NIP incorrecto. Te quedan 1 intentos.
Ingresa tu NIP: 3333
NIP incorrecto. Te quedan 0 intentos.
Tarjeta bloqueada por seguridad
```
