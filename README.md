# 🧪 Laboratorio #2 - Implementación de Login en Laravel

## 📌 Introducción

El presente laboratorio tiene como objetivo implementar un sistema de autenticación (login) utilizando el framework Laravel, aplicando la arquitectura Modelo-Vista-Controlador (MVC).

Laravel organiza sus componentes de la siguiente manera:

* **Modelos (Models):** Gestionan la lógica de negocio y la interacción con la base de datos.
* **Vistas (Views):** Representan la interfaz gráfica del sistema.
* **Controladores (Controllers):** Procesan las solicitudes del usuario y conectan modelos con vistas.
* **Rutas (Routes):** Definen las direcciones URL y su comportamiento.

El objetivo principal fue configurar un entorno funcional, instalar dependencias y lograr un sistema de login operativo.

---

## ⚙️ Requisitos Previos

Para ejecutar el proyecto se requiere:

* PHP 8.0 o superior
* Composer
* Laravel
* Servidor local (WampServer / XAMPP / Laragon)
* Apache o Nginx
* MySQL o MariaDB
* Visual Studio Code

---

## 🚀 Instalación del Proyecto

### 1. Crear proyecto Laravel

```bash
composer create-project laravel/laravel mi_proyecto
cd mi_proyecto
```

### 2. Instalar dependencias

```bash
composer install
```

### 3. Configurar archivo .env

```bash
cp .env.example .env
php artisan key:generate
```

### 4. Instalar sistema de autenticación (Laravel Breeze)

```bash
composer require laravel/breeze --dev
php artisan breeze:install
npm install
npm run dev
```

### 5. Ejecutar migraciones

```bash
php artisan migrate
```

### 6. Ejecutar servidor

```bash
php artisan serve
```

Acceso al sistema:
http://127.0.0.1:8000/

---

## 🗄️ Base de Datos

Se utilizó MySQL como sistema gestor de base de datos.

Configuración en el archivo `.env`:

```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=
DB_USERNAME=root
DB_PASSWORD=
```

Comando ejecutado para crear las tablas:

```bash
php artisan migrate
```

Tablas creadas automáticamente:

* users
* password_reset_tokens
* sessions

Se incluye en el repositorio un respaldo de la base de datos (.sql).

---

## 🖼️ Resultado del Laboratorio

El sistema permite:

* Registro de usuarios
* Inicio de sesión
* Cierre de sesión


---

## ⚠️ Dificultades y Soluciones

**Problema 1:** Error al ejecutar `php artisan serve`
**Solución:** Se verificó la instalación de PHP y se corrigió la configuración del PATH.

**Problema 2:** Error al cargar dependencias
**Solución:** Se ejecutó `composer install` correctamente.

**Problema 3:** Problemas con el archivo `.env`
**Solución:** Se configuraron correctamente los datos de conexión a la base de datos.

**Problema 4:** Error con npm
**Solución:** Se ejecutó `npm install` y `npm run dev`.

---



## 📅 Fecha de Ejecución

Abril 15 2026

---

## 👨‍💻 Información del Estudiante

Este laboratorio ha sido desarrollado por el estudiante de la Universidad Tecnológica de Panamá:

* Nombre: Andrea Torrrento 
* Correo: andrea.torrento@utp.ac.pa
* Curso: Desarrollo de Software VII
* Instructor: Ing. Irina Fong
