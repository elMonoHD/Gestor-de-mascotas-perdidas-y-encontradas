# Gestor-de-mascotas-perdidas-y-encontradas
1.- Descripción breve del sistema:

El Gestor de Mascotas Perdidas y Encontradas es una aplicación web que permite registrar y visualizar mascotas que han sido reportadas como perdidas o encontradas.

El sistema permite:

1.1.- Crear una mascota con nombre, raza y foto.

1.2.- Se publican las mascotas registradas recientemente en el home

1.3.- Formulario para registrar mascotas

1.4.- Formulario para agregar una nueva publicación

1.5.- Se visualizan todos los datos de todas las mascotas, perdidas y encontradas

1.6.- Se visualizan los detalles de cada publicación y para gestionar las mascotas registradas

1.7.- Sistema de crud basico que permite crear, editar, leer, eliminar y actualizar.

1.8.- Su objetivo es facilitar que personas puedan reportar y encontrar mascotas de forma rápida y organizada.

2.-Diagrama de los modelos y sus relaciones:

Relación entre las tablas del backend (Django):

Mascota:

id (automático)

nombre: texto

Raza: texto

foto: imagen

Relación uno a muchos (una mascota → una publicación)

Publicación:

id

mascota (ForeignKey a Mascota)

tipo (perdida o encontrada)

descripcion

lugar

fecha (automática)

contacto 

encontrada (True/False)


3.- Capturas de pantalla del frontend funcionando en un word, almacenado en el winrar del proyecto "Gestor-mascotas".


4.- Instrucciones para ejecutar el backend y el frontend

Backend:

1.	En la consola del visual situarse en la carpeta del proyecto mediante con un “cd gestor_mascotas_backend”
2.	Activar el entorno virtual mediante el comando “pipenv shell”
3.	Instalar django rest framework mediante el comando “pip install djangorestframework”
4.	Instalar pillow con el comando “pip install pillow”
5.	Correr el servidor con el comando “python manage.py runserver”
6.	En la url escribir /api 

Frontend:
1.	Situarse en la carpeta del proyecto mediante un “cd gestor_mascotas_frontend”
2.	Correr el servidor mediante con el comando “npm start”
