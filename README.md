# koyag_test
* ¿Qué es un Eloquent Model y cómo lo usarías para consultar datos en una tabla?
Eloquent es el ORM usado por Laravel para trabajar con bases de datos utilizando objetos PHP, por tanto Eloquent Model es una clase que representa una tabla o entidad de la base de datos y proporciona una forma orientada a objetos para interactuar con los datos de esa tabla.

Suponiendo que desea crea una tabla users, se puede crear un modelo llamado Users con el siguiente comando:

```
php artisan make:model User
```
Para consultar datos de la tabla > users
```
use App\Models\User;

// Obtener todos los registros
$users = User::all();

// Obtener un registro específico por ID
$post = User::find(1);
```

* Bases de Datos (MySQL):
Consulta SQL para contar usuarios activos:
```
SELECT COUNT(*) AS active_users FROM users WHERE status = 'active';
```

* APIs RESTful:
Explica brevemente qué son los status codes en una API REST y menciona al menos tres códigos comunes con su significado.

Los códigos de estado es la forma en que una API REST usa para informar al usuario sobre el resultado de su solicitud, indicando si la solicitud fue exitosa o si tuvo algún error.

200 OK: solicitud exitosa
404 Not Found: el recurso no existe
500 Internal Server Error: hubo un error interno en el servidor al ejecutar la solicitud