# Levantar ambiente de desarrollo

En la raiz del directorio se debe ejecutar el comando:

 ```php
    docker-compose up -d --build
```
Para poder construir el contener con apache, php-8, composer y las dependencias de SQL Server

Una vez finalizado esto se debe correr el comando
```php
    docker-compose exec php-apache /bin/bash
```

Para acceder en modo interactivo al contenedor donde estara viviendo el proyecto dentro de la carpeta src/

En caso de dar problemas con los permisos en storags/logs se debe correr el comando:
```php
    chmod 777 -R storage bootstrap public
```
Para darle permisos de escritura y lectura a todos los archivos.



## License

The Laravel framework is open-source software licensed under the [MIT license](https://opensource.org/licenses/MIT).