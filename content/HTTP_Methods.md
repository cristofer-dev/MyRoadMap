## HTTP Methods 

### `GET`
- `user/2` OBTENER item con `id 2`
- `user` OBTENER todos los items

### `PUT`
- `user/5` MODIFICAR el usuario con `id 5`
- `user/12/order/456` MODIFICAR la `orden 456` del `usuario 5`

### `PATCH`
- `user/5` MODIFICAR el usuario con `id 5`
- `user/12/order/456` MODIFICAR la `orden 456` del `usuario 5`

### `DELETE`
- `user/5` ELIMINAR el usuario con `id 5`
- `user/12/order/456` ELIMINAR la `orden 456` del `usuario 5`
- `user/12/order/` ELIMINAR las todas las `ordenes` del `usuario 5`

### `POST`
- `user/` CREAR el usuario con `id 5`
- `user/12/order/456` CREAR una nueva `orden` para el `usuario 5`
