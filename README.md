# QA Engineer Lab

Proyecto personal para practicar habilidades de QA Engineer.

Incluye:

- API Testing
- Automatización
- Microservicios
- CI/CD con Jenkins

Tecnologías:

- Postman
- Node.js
- Express
- GitHub
- Jenkins

# QA Engineer API Testing Lab

Proyecto de laboratorio para practicar pruebas de API y automatización.

## Tecnologías utilizadas

- Postman
- Newman
- Node.js
- Express.js

## Escenario

Se desarrolló un microservicio simple de usuarios y se realizaron pruebas automatizadas sobre sus endpoints.

Endpoints probados:

GET /users  
GET /users/:id  
POST /users  

## Ejecución del microservicio

cd user-service  
node server.js

## Ejecutar pruebas automatizadas

newman run api-testing/user-service-tests.postman_collection.json

## Generar reporte

newman run api-testing/user-service-tests.postman_collection.json -r html --reporter-html-export newman/user-service-report.html

## Resultados

Los tests validan:

- Status codes
- Estructura JSON
- Creación de usuarios
- Manejo de errores (404)


Autor:
Juan Felipe Betancourt
QA Engineer