# Traspaso

## Qué cambió

- Se agregó a `reglas.md` la regla 4: «Un ejecutivo no puede tener más de 18 clientes». Está en la rama `regla-tope-18-clientes`, en un pull request que todavía no se fusiona.

## Qué quedó pendiente

- Otra persona tiene que revisar el pull request antes de aceptarlo (todo cambio a `reglas.md` lo exige).
- Con los datos de hoy (`datos/carteras_clientes.csv`), dos ejecutivos pasan el tope: E6 tiene 24 clientes y E3 tiene 19. Falta decidir cómo se reparten esos 7 clientes de más. La regla 3 dice que cada reasignación necesita la aprobación del jefe comercial.

## Qué decidimos y por qué

- Las reglas no ponían ningún límite a la cantidad de clientes por ejecutivo, y con eso las carteras quedaban muy desparejas (de 11 a 24 clientes). El número 18 fue lo que se pidió y coincide con la capacidad más alta que figura en `datos/carteras_ejecutivos.csv` (E2). El motivo de negocio de ese número no está escrito en ninguna parte.

## Qué no hay que tocar

- `main`: se cambia solo a través de un pull request.
- Las reglas 1 a 3 siguen como estaban.

## Cuál es el siguiente paso

- Revisar y aprobar el pull request y después reasignar los clientes de más que tienen E6 y E3.
- Falta definir qué pasa si un cliente de más de $10M (regla 2) tiene que ir a un ejecutivo senior y ningún senior tiene espacio bajo el tope.
