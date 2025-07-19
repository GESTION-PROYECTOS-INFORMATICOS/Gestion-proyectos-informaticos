# Gestion-proyectos-informaticos


##Introducción##
Este repositorio está dedicado a la gestión del proyecto informático, documentando las configuraciones, reglas y procesos necesarios para el desarrollo y la colaboración del equipo. Aquí encontrarás las pautas para contribuir y mantener la coherencia en el proyecto.

##Reglas de contribución##
1. Ramas independientes por funcionalidad o arreglo. Cada vez que se agrega una nueva función o se arregla un bug, debe hacerse en una rama nueva con prefijo:
feature/ para nuevas funciones
fix/ para arreglos normales o urgentes
Ejemplo: feature/login-form, fix/navbar-alignment

2.No se permiten merges directos a la rama main sin un pull request (PR) aprobado 
por otro integrante. 

3. Cada versión funcional del sistema debe marcarse con un tag semántico (v1.0.0, 
v1.1.0, etc.).
 


###Evidencias###
*Imagen de Postman
https://imgur.com/a/dMJmnFf

# COMO EJECUTAR EL PRODUCTO
Requisitos previos:
* Node.js (versión recomendada: 18.x o superior)
* npm (incluido con Node.js)
* .NET SDK (versión recomendada: 7.0 o superior)

- Crear una carpeta (por ejemplo: GPI_WEB)
- Clonar dentro de la misma https://github.com/GESTION-PROYECTOS-INFORMATICOS/Frontend.git
- Clonar dentro de la misma https://github.com/GESTION-PROYECTOS-INFORMATICOS/Backend.git
  
Para ejecutar front-end:
* Estar dentro del directorio "frontgestion"
* instalar dependencias: npm i
* ejecutar comando: npm run dev
  
Para ejecutar back-end:
* Estar dentro del directorio "backGestion"
* ejecutar comando: dotnet run
  
Nota importante: Para que el front funcione, se debe crear un archivo .env.local al mismo nivel del directorio "frontgestion", el contenido de ese archivo son credenciales que por seguridad no se encuentran dentro de este proyecto. De ser necesarias, solicitarlas a cualquier integrante del proyecto. 

Consideraciones adicionales: Asegurarse de que tanto el frontend como el backend estén corriendo simultáneamente para que la aplicación funcione correctamente.
El frontend se conectará automáticamente al backend según las variables definidas en .env.local.

