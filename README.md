# laravel_notes
apuntes a cerca de laravel

<h1>Resetear base de datos y actualizar las tablas</h1>

```
php artisan migrate:fresh
```

<h1>Poder acceder a la carpeta storage, esto se usa cuando subes imagenes al proyecto</h1>

```
php artisan storage:link
```

<h1>Crear un modelo, controlador y migracion al mismo tiempo</h1>

```
php artisan make:model -mrc nombre_del_recurso
```

<h1>Crear un modelo y migraciones</h1>

```
php artisan make:model nombre_del_recurso -m
```

<h1>Para permitir recibir solicitudes se tiene que agregar la url de la aplicacion en el siguiente archivo </h1>

```
App\Http\Middleware\VerifyCsrfToken
```
<p>Agregar el siguiente codigo</p>

```
protected $except = [
        '/urlDelArchivo',
    ];
```

<p>Funcion que automatiza el entorno de desarrollo con laravel y npm en powershell</p>

```
function Work {
    $dirPath = "Aqui va el directorio de trabajo"
    Start-Process powershell -ArgumentList "-NoExit", "-Command", "cd $dirPath; php artisan serve" 
    Start-Process powershell -ArgumentList "-NoExit", "-Command", "cd $dirPath; npm run dev" 
    Start-Process powershell -ArgumentList "-NoExit", "-Command", "cd $dirPath" 
}
```

