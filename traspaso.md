# Traspaso

## Qué cambió

- Se unió `main` en `agente-b`. El conflicto estaba en la regla 4 de `reglas.md`: `main` ponía el tope en 18 clientes y `agente-b` en 20.
- Se dejó 18. Con eso, `agente-b` ya no cambia nada de `reglas.md` respecto de `main`.

## Qué quedó pendiente

- Hoy, según `datos/carteras_clientes.csv`, pasan el tope de 18 dos ejecutivos: E6 (24 clientes) y E3 (19). Falta definir cómo se les reasignan clientes (la regla 3 pide la aprobación del jefe comercial).
- No está definido qué hacer cuando las reglas 1 o 2 indican un ejecutivo que ya tiene 18 clientes.

## Qué decidimos y por qué

- Tope de 18. Ya estaba aprobado en `main` (PR 4) y coincide con la capacidad más alta de `datos/carteras_ejecutivos.csv` (E2). El 20 no tenía fundamento en los datos.

## Qué no hay que tocar

- La regla 4 de `reglas.md`. Para cambiarla hay que abrir un PR propio, y otra persona tiene que revisarlo.

## Cuál es el siguiente paso

- Decidir si el tope debería ser la `capacidad_clientes` de cada ejecutivo en vez de un número fijo: casi todos tienen capacidad 14 o 16, por debajo de 18. Si se decide que sí, va en un PR aparte con revisión.
