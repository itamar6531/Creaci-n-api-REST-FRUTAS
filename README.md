# Creacion-api-REST-FRUTAS
Objetivo: Aplicar los conocimientos sobre desarrollo de APIs REST utilizando un framework backend (ej. Laravel) para construir un CRUD funcional con relaciones y lógica de negocio.

En este repositorio se incluirá en código fuente del proyecto hecho con Laravel framework y testeado con POSTMAN. 
La creación de la base de datos fue levantada en XAMPP, por ende, para probar el proyecto se debe instalar XAMPP para tener acceso a phpMyAdmin. El proyecto debe ser instalado en \xampp\htdocs.
En phpMyAdmin, crear una base de datos 'frutas_db' y despues ejecutar las migraciones y el seeder:
* php artisan migrate
* php artisan db:seed

Iniciar el servidor con: php artisan serve, y con postman probar si el servidor responde con un metodo GET hacia esta direccion: http://localhost:8000/api/test. Le deberia salir un mensaje indicando que la API Frutas funciona correctamente.

Para probar el recurso en Postman:
* GET hacia la direccion http://localhost:8000/api/categorias, para obtener todas las categorias
* GET hacia la direccion http://localhost:8000/api/frutas/1, para obtener la fruta con ID 1
* POST hacia la direccion http://localhost:8000/api/categorias, seleccionar Body en formato JSON con el cuerpo:
  {
    "nombre": "Frutos Secos"
  ]
  Para crear una nueva categoria 'Frutos Secos'
* PUT hacia la direccion http://localhost:8000/api/frutas/1, con cuerpo en formato JSON: {
    "nombre": "Mango Naranja",
    "color": "Amarillo",
    "fecha_cosecha": "2025-06-18"
    ]
  Para actualizar la fruta con ID #1.
* DELETE hacia la direccion http://localhost:8000/api/frutas/1, para eliminar la fruta con ID #1.



