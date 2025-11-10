Proyecto Backend con Node.js, Express y PostgreSQL

Este proyecto implementa un servidor backend utilizando Node.js, Express y PostgreSQL. 
Expone una API REST básica para gestionar usuarios (crear y listar). Está diseñado como 
base para integrarse con un frontend en React u otras aplicaciones.

REQUISITOS:
- Node.js instalado (versión 14+ recomendada)
- PostgreSQL instalado y corriendo
- Postman (opcional)

INSTALACIÓN:
1. Ejecutar: npm install
2. Configurar db.js con tus credenciales de PostgreSQL
3. Crear la Base de Datos:
   CREATE DATABASE usuarios_db;
   CREATE TABLE usuarios (
     id SERIAL PRIMARY KEY,
     nombre VARCHAR(50),
     correo VARCHAR(100),
     contraseña VARCHAR(100)
   );

EJECUCIÓN:
npm start
Servidor disponible en http://localhost:3000

ENDPOINTS:
GET /  -> Prueba del servidor
POST /usuarios  -> Crear usuario
GET /usuarios   -> Listar usuarios

MEJORAS A FUTURO:
- Validación de datos
- Encriptación de contraseñas
- Login con JWT
- CRUD completo
