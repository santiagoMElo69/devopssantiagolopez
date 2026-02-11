# devopssantiagolopez
Proyecto en Java que implementa una API básica para la gestión de Estudiantes, usando el patrón MVC y un pipeline de Integración Continua con GitHub Actions.
Los datos se almacenan en memoria y no se utiliza base de datos.

# Endpoints
## Crear estudiante

POST /estudiantes
- Registra un estudiante validando que el id no se repita.
Respuesta: 201 Created

## Listar estudiantes

GET /estudiantes
- Devuelve todos los estudiantes registrados.
Respuesta: 200 OK

# Control de Versiones

Se utiliza GitFlow:

main: rama estable

development: rama de desarrollo
La integración se realiza mediante Pull Requests.

# CI

El proyecto cuenta con un pipeline en GitHub Actions que:

- Compila el proyecto automáticamente

- Se ejecuta en cada push y pull request

- Genera un GitHub Release al hacer merge a main

# Tecnologías

- Java

- Gradle

- GitHub Actions

- GitFlow 
