# Edusphere

Este proyecto es una plataforma escolar completa desarrollada con Laravel 11 para el backend y React 19 con TypeScript y Tailwind CSS 4 para el frontend.

## Tecnologías Utilizadas

- **Backend**: Laravel 11 (PHP 8.2)
- **Frontend**: React 19 con TypeScript
- **Base de Datos**: MySQL
- **Autenticación**: Laravel Sanctum
- **Estilos**: Tailwind CSS 4
- **Gestión de Calendario**: FullCalendar.js

## Configuración del Backend (Laravel 11)

1. **Requisitos Previos:**
   - PHP 8.2 o superior
   - Composer
   - MySQL 8 o MariaDB
   - Node.js y npm

2. **Instalación**:
   ```bash
   composer create-project laravel/laravel backend
   cd backend
   php artisan serve

3. **Configuración de la Base de Datos:**
   Modifica el archivo .env con tus credenciales de MySQL

4. **Migraciones**:
   Ejecuta las migraciones para crear las tablas necesarias:
   ```bash
   php artisan migrate

5. **Seeders**:
   Ejecuta los seeders para poblar la base de datos con datos de prueba:
   ```bash
   php artisan db:seed

6. **Autenticación con Laravel Sanctum**:
   - Instala Sanctum: *composer require laravel/sanctum*
   - Publica la configuración de CORS: *php artisan config:public cors*
   - Configura *config/cors.php* para permitir las solicitudes desde tu frontend

## Configuración del Frontend (React 19)

1. **Requisitos Previos**:
   - Node.js
   - npm

2. **Instalación**:
   ```bash
   cd frontend
   npm create vite@latest -- --template react-ts
   npm install
   npm install tailwindcss @tailwindcss/vite

3. **Configuración de Tailwind CSS 4**
   - Configura *vite.config.ts* para usar Tailwind CSS.
   - Importa Tailwind CSS en *src/index.css*: *@import "tailwindcss";*

4. **Ejecutar el Frontend**:
   ```bash
   npm run dev

## Configuración del Backend (Laravel 11)

  - **Autenticación**: Registro, inicio de sesión y cierre de sesión de usuarios mediante laravel Sanctum.
  - **Gestión de Usuarios**: Administración de roles (admin, profesor, estudiante) y permisos.
  - **Gestión Académica**:
      - Cursor y asignaturas
      - Tareas y evalucaciones
      - Asistencia y calendario de eventos
  - **Comunicación**: Mensajería interna y notificaciones.
  - **Auditoría**: Registro de actividades y errores del sistema.
