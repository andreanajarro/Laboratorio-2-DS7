# 📌 Instalación de Laravel - Proyecto

## 🧾 Descripción

En este proyecto se realizó la instalación y configuración de un entorno de desarrollo para trabajar con Laravel. Se utilizó WAMP como servidor local, Composer para la gestión de dependencias y Node.js para la compilación de recursos frontend. Finalmente, se implementó el sistema de autenticación (Login y Register).

---

## ⚙️ Tecnologías utilizadas

* PHP (8.5)
* Laravel
* Composer
* Node.js y npm
* WAMP Server

---

## 🚀 Pasos realizados

1. Instalación de WAMP Server.
2. Instalación de Composer.
3. Configuración de PHP (actualización a versión compatible).
4. Creación del proyecto Laravel:

   ```
   composer create-project laravel/laravel mi_proyecto
   ```
5. Configuración del archivo `.env`.
6. Ejecución de migraciones:

   ```
   php artisan migrate
   ```
7. Instalación de autenticación:

   ```
   composer require laravel/ui
   php artisan ui bootstrap --auth
   ```
8. Instalación de dependencias frontend:

   ```
   npm install
   npm run dev
   ```
9. Ejecución del servidor:

   ```
   php artisan serve
   ```

---

## 🔐 Resultado

Se logró implementar correctamente:

* Registro de usuarios
* Inicio de sesión (Login)
* Conexión con base de datos SQLite
* Interfaz básica con Bootstrap

---

## ⚠️ Problemas encontrados y soluciones

### ❌ 1. Error de versión de PHP

**Problema:** Laravel requería una versión más reciente de PHP.
**Solución:** Se instaló y configuró PHP 8.5 en WAMP.

---

### ❌ 2. Comando `php` no reconocido

**Problema:** El sistema no reconocía el comando `php`.
**Solución:** Se agregó la ruta de PHP a las variables de entorno (PATH).

---

### ❌ 3. Error de dependencias en Composer

**Problema:** No se podían instalar paquetes por incompatibilidad.
**Solución:** Se actualizó PHP a una versión compatible.

---

### ❌ 4. Carpeta del proyecto ya existente

**Problema:** Laravel no permitía crear el proyecto porque la carpeta no estaba vacía.
**Solución:** Se eliminó la carpeta y se volvió a ejecutar el comando.

---

### ❌ 5. Error con Node.js (`npm no reconocido`)

**Problema:** No se podía ejecutar `npm install`.
**Solución:** Se instaló Node.js y se verificó su configuración en PATH.

---

### ❌ 6. Bloqueo de firewall de Windows

**Problema:** Windows bloqueó Node.js al ejecutar `npm run dev`.
**Solución:** Se permitió el acceso en redes privadas.

---

### ❌ 7. Error `Could not open input file: artisan`

**Problema:** Se ejecutaba el comando fuera del directorio del proyecto.
**Solución:** Se navegó a la carpeta correcta antes de ejecutar comandos.

---

### ⚠️ 8. Advertencia de Xdebug

**Problema:** Mensaje de error al cargar Xdebug.
**Solución:** Se ignoró ya que no afecta el funcionamiento del proyecto.



## 🧠 Conclusión

Se logró configurar correctamente el entorno de desarrollo para Laravel, resolviendo distintos problemas técnicos durante la instalación. El sistema de autenticación funciona correctamente, permitiendo el registro e inicio de sesión de usuarios.


## 📎 Notas

Este proyecto se ejecuta en entorno local utilizando:


http://127.0.0.1:8000

