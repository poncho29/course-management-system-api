<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Prueba Técnica Junior: Sistema de Gestión de Curso

## Obejtivo:
Construir una aplicación para gestionar un curso y sus estudiantes, permitiendo crear, actualizar y eliminar un curso, así como añadir y remover estudiantes. La aplicación debe incluir una funcionalidad personalizada para calcular un índice de diversidad basado en los dominios de los emails de los estudiantes.

## Tecnologías Utilizadas:
- NestJS
- TypeORM
- PostgreSQL

## Instrucciones de Instalación:
1. Instalar dependencias:
``` npm install ```

2. Configurar variables de entorno agregando el archivo ```.env``` adjunto.

3. Iniciar el servidor:
``` npm run start:dev ``` 

## Funcionalidad de la API:

### Modulo de Cursos:
- Listar todos los cursos con indice de diversidad (GET /courses)
- Listar un curso (GET /courses/:id)
- Crear un curso (POST /courses)
- Actualizar un curso (PUT /courses/:id)
- Eliminar un curso (DELETE /courses/:id)
- Listar estudiantes de un curso (GET /courses/students?courseId=)
- Agregar un estudiante a un curso (POST /courses/students)
- Eliminar un estudiante de un curso (DELETE /courses/students/:id) se elimina con el id de la relacion curso_estudiante

### Modulo de Estudiantes:
- Listar todos los estudiantes (GET /students)
- Listar un estudiante (GET /students/:id)
- Crear un estudiante (POST /students)
- Actualizar un estudiante (PUT /students/:id)
- Eliminar un estudiante (DELETE /students/:id)

