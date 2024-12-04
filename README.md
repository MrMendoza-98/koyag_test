# koyag_test
¿Qué es un Eloquent Model y cómo lo usarías para consultar datos en una tabla?
Eloquent es el ORM usado por Laravel para trabajar con bases de datos utilizando objetos PHP, por tanto Eloquent Model es una clase que representa una tabla o entidad de la base de datos y proporciona una forma orientada a objetos para interactuar con los datos de esa tabla.

Suponiendo que desea crea una tabla users, se puede crear un modelo llamado Users con el siguiente comando:

```
php artisan make:model User
```
Para consultar datos de la tabla > users

use App\Models\User;

// Obtener todos los registros
$users = User::all();

// Obtener un registro específico por ID
$post = User::find(1);