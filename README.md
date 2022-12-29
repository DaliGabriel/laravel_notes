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

