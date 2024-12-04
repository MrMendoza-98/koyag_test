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

* Control de Versiones (Git):
Describe los pasos básicos para crear una nueva rama, trabajar en ella y luego fusionarla con la rama principal (main o master).

Crear una rama en git 
```
git checkout -b feature/new-branch
```
Registrar los cambios en el código, y agrega y confirma los cambios
```
git add .
git commit -m "feat: changes"
```
Cambiar a la rama principal (main o master)
```
git checkout main
```
Fusionar la nueva rama con la principal
```
git merge feature/new-branch
```
Eliminar la rama después de la fusión
```
git branch -d feature/new-branch
```
* ¿Qué harías si te asignan una tarea técnica que no sabes cómo resolver?

Para atender una tarea técnica que no sé como resolver realizaría los siguientes pasos:

- Entender el problema:
Recepcionar la tarea o problema.
Identificarlos objetivos y entender los posibles impedimento o restricciones.
Preguntar si no es claro los requerimientos para evitar perdida de tiempo y malentendidos.

- Investigar
Buscar en la documentación oficial de las tecnologías si no tengo conocimientos técnicos de como realizar la tarea.
Revisar tutoriales o recursos confiables.
Si la tarea involucra código existente, analizarlo para entender cómo funciona.

- Dividir la tarea en partes más pequeñas
Si la tarea es muy compleja se dividen en subtareas para de esa forma sea manejable.

- Solicitar ayuda si la necesito
Consultar con compañeros, expertos en el tema o el equipo técnico.

- Validar el resultado
Asegurar que la solución implementada cumple con los requerimientos iniciales.
Realizar pruebas para verificar la funcionalidad, rendimiento y posibles errores.

- Comunicar los avances
Mantener a las personas o equipo informado sobre los avances y cualquier obstáculo encontrado.