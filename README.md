# Desafío Backend Node.js

¡Bienvenido al desafío backend Monbak.

En este desafío, tu tarea es crear un servidor backend utilizando Node.js que tenga un endpoint para cada verbo HTTP (GET, POST, PUT, DELETE) y que utilice un middleware básico de autenticación.

## Requisitos para Completar el Desafío

Para completar este desafío, debes tener los siguientes requisitos en tu máquina local:

1. **Node.js y npm**:

   - Verifica si están instalados ejecutando los siguientes comandos en tu terminal:
     ```bash
     node -v
     npm -v
     ```
   - Si no están instalados, descárgalos e instálalos desde [Node.js official website](https://nodejs.org/).

2. **Editor de código**:

   - Recomendado: Visual Studio Code, Sublime Text o Atom.
   - Descarga Visual Studio Code desde [Visual Studio Code](https://code.visualstudio.com/).

3. **Postman o cURL**:

   - Para probar tus endpoints, utiliza Postman (descargable desde [Postman official website](https://www.postman.com/)) o cURL.

4. **Git**:
   - Verifica si Git está instalado ejecutando el siguiente comando:
     ```bash
     git --version
     ```
   - Si no está instalado, descárgalo e instálalo desde [Git official website](https://git-scm.com/).

## Instrucciones

1. Clona este repositorio en tu máquina local.

2. Implementa los siguientes requisitos:

   - Crea un archivos `server.js`. Este archivo será el punto de entrada de la aplicación.

   - Crea un archivo `routes.js` donde definirás y configurarás los endpoints utilizando un router de Express.
   - Utiliza el router de Express para gestionar las rutas y los controladores asociados a cada endpoint.
   - Implementa un endpoint para cada verbo HTTP (GET, POST, PUT, DELETE):

     - `GET /api` : Retorna un mensaje de bienvenida al API.
     - `GET /api/task`: Retorna todos los recursos disponibles.
     - `POST /api/task`: Crea un nuevo recurso.
     - `PUT /api/task/:id`: Actualiza un recurso existente.
     - `DELETE /api/task/:id`: Elimina un recurso por su ID.

   - Intenta estructurar tu código usando el patron de capas Layered Pattern.
   - Asegúrate de que los códigos de respuesta HTTP sigan las normas actuales y sean apropiados para cada situación.
   - Configura el middleware de CORS (Cross-Origin Resource Sharing) para permitir las solicitudes desde dominios específicos.
   - Utiliza un middleware básico de autenticación para proteger tus endpoints (El endpoint `/api` debe estar libre de protección). Puedes usar, por ejemplo, un token de autenticación enviado en la cabecera de la solicitud (header). En este punto no es neceario implementar un sistema de autenticación completo, simplemente verifica que el token sea válido y que el usuario tenga permisos para acceder a los recursos solicitados.
   - Asegúrate de que las respuestas del API incluyan el header `Content-Type: application/json`.
   - Utiliza el archivo `db.json` en la raíz del proyecto como base de datos local para almacenar los datos. Este archivo debe ser leído y escrito por los endpoints según sea necesario.
   - El servidor debe correr en el puerto `8264`

3. Prueba tu aplicación utilizando herramientas como Postman o cURL para asegurarte de que los endpoints funcionan correctamente y que el middleware de autenticación está protegiendo los recursos de manera adecuada.

4. Una vez completado, sube tu solución al repositorio (o enviala en formato .zip) y asegúrate de crear un archivo `INSTRUCTIONS.md` con instrucciones claras sobre cómo ejecutar y probar tu aplicación.

¡Buena suerte!

## Recursos útiles

- Documentación oficial de Node.js: [Node.js Docs](https://nodejs.org/en/docs/)
- Documentación de Express.js: [Express.js Docs](https://expressjs.com/)
- Mdn web docs HTTP: [Http response status codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)
- Tutorial sobre middleware de autenticación en Express.js: [Express.js Authentication Middleware Tutorial](https://www.digitalocean.com/community/tutorials/nodejs-jwt-expressjs)
- Arquitectura de capas en Nodejs: [Layered Architecture for NodeJs](https://ctrly.blog/nodejs-layered-architecture/)
