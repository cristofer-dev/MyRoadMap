## ApiRest

### Recomendaciones Generales
- Debe ser fácil de usar y hacer la vida del desarrollador mas "suave"

### Terminos
- `Recurso` : Es un sustantivo, que representa por lo general un objeto o actor del sistema,
- `colección` : Conjunto de recursos
- `metodo` : Es un verbo o accion que eventualmente se le asocia a un recurso.

## HTTP Methods 

### `GET`
- `users/2` OBTENER item con `id 2`
- `users` OBTENER todos los usuario
- `companies/3/users` OBTENER todos los usuarios de la compañia `3`
- `companies/3/users/4` OBTENER el usuario `4` de la compañia `3`

### `POST`
- `user/` CREAR un usuario
- `user/12/order/456` CREAR una nueva `orden` para el `usuario 12`

### `PUT`
- `user/5` MODIFICAR el usuario con `id 5`
- `user/12/order/456` MODIFICAR la `orden 456` del `usuario 12`

### `DELETE`
- `user/5` ELIMINAR el usuario con `id 5`
- `user/12/order/456` ELIMINAR la `orden 456` del `usuario 12`
- `user/12/order/` ELIMINAR las todas las `ordenes` del `usuario 12`

### `PATCH`
- `user/5` MODIFICAR el usuario con `id 5`
- `user/12/order/456` MODIFICAR la `orden 456` del `usuario 12`

## HTTP Response

### `2xx` (success)

- `200`: Ok
- `201`: Created
- `204`: Completado, pero no retorna resultado ( ej. DELETE )

### `4xx` (client error)

- `400`: Bas Request, el servidor no puede entener lo que el cliente pide.
- `401`: Unauthorize, el recurso existe, pero el clinete no tiene permisos para usarlo.
- `403`: Forbidden, el recurso existe, el cliente tiene los permisos (de api), pero por alguna razon no tiene permisos para acceder a la pagina (por lo general configuracion de permisos a nivel de servidor web).
- `404` : Not Found, el recurso no esta disponible por ahora.
- `410` : Gone, el recurso ha sido movido intencionalmente.

### `5xx` (server error)

- `500`: Internal server error, Recurso valido, pero ocurrio una condición inesperada.
- `503`: Service unavailable, servidor apagado o no disponible.

## Searching, sorting, filtering and pagination

- **Sorting**
  - `GET /companies?sort=rank_asc` 
- **Filtering**
  - `/companies?category=banking&location=india`
- **Searching**
  - `/companies?search=Digital Mckinsey`
- **Pagination**
  - `/companies?page=23`

## Versionado

- `http://api.yourservice.com/v1/companies/34/employees ` : version 1
- `http://api.yourservice.com/v2/companies/34/employees ` : version 2
- `http://api.yourservice.com/v2.2/companies/34/employees ` : version 2.2
