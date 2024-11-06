<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

# Laravel Blog

Este es un proyecto de blog desarrollado con **Laravel**. El proyecto no solo expone una API, sino que también incluye un frontend utilizando **Blade** como motor de plantillas. El backend proporciona las funcionalidades de la API, mientras que el frontend se encarga de la visualización de datos utilizando vistas de Blade.

## Requisitos

- PHP >= 8.0
- Composer
- MySQL
- Node.js y npm

## Instalación

1. Clona el repositorio a tu máquina local:
```bash
   git clone <URL DEL REPOSITORIO>
   cd laravel_blog
```
2. Instala las dependencias de PHP:
```bash
    composer install
```

3. Instala las dependencias de PHP:
```bash
    composer install
```

4. Copia el archivo .env.example a un archivo .env:
```bash
    cp .env.example .env
```

5. Genera la clave de la aplicación de Laravel:
```bash
    php artisan key:generate
```

6. Configura tu base de datos en el archivo .env. Asegúrate de tener una base de datos de MySQL creada y actualiza las siguientes variables con la configuración adecuada:
```bash
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=nombre_de_tu_base_de_datos
    DB_USERNAME=tu_usuario
    DB_PASSWORD=tu_contraseña
```

7. Ejecuta las migraciones para crear las tablas en la base de datos:
```bash
    php artisan migrate
```

8. Opcional) Si deseas poblar la base de datos con datos de prueba, puedes usar las factories de Laravel. Asegúrate de tener configurados los archivos de factory y luego ejecuta:
```bash
    php artisan db:seed
```
9. Inicia el servidor de desarrollo de Laravel:
```bash
    php artisan serve
```

9. Comando para compilar los archivos CSS y JavaScript con Vite y Tailwind CSS (debe ejecutarlo en una consola a parte dentro del proyecto):
```bash
    npm run dev
```

## Comandos utilies

* Ejecutar migraciones: Para crear las tablas en la base de datos:
```bash
php artisan migrate
```

* Revertir migraciones: Para revertir la última migración ejecutada:
```bash
php artisan migrate:rollback
```

* Revertir todas las migraciones: Para revertir todas las migraciones:
```bash
php artisan migrate:reset
```

* Revertir y volver a ejecutar migraciones: Para revertir las migraciones y luego volver a ejecutarlas:
```bash
php artisan migrate:refresh
```

* Forzar migración en producción: Si necesitas forzar la ejecución de migraciones en un entorno de producción (para evitar la confirmación de la migración):
```bash
php artisan migrate --force
```

* Poblar la base de datos con datos de prueba: Para ejecutar los seeders y poblar la base de datos con datos de prueba:
```bash
php artisan db:seed
```

* Ejecutar un seeder específico: Si quieres ejecutar un seeder específico:
```bash
php artisan db:seed --class=NombreDelSeeder
```
