# MERN Calendar Backend

Este es el backend de una aplicación de calendario construida con el stack MERN (MongoDB, Express, React, Node.js). La aplicación incluye autenticación y CRUD de eventos.

## Requisitos

- Node.js
- MongoDB

## Instalación

1. Clona el repositorio:
    ```sh
    git clone https://github.com/MatiasCutri/CalendarApp.git
    cd CalendarApp
    ```

2. Instala las dependencias:
    ```sh
    npm install
    ```

3. Configura las variables de entorno:

    - Clonar el archivo `.env.template`, renombrarlo a `.env` y cambiar las variables de entorno acorde a tu configuración
        ```properties
        PORT=4000
        DB_CNN=mongodb+srv://mern_user:GGKA7EU80G4eHfSd@calendardb.b1cyf.mongodb.net/mern_calendar
        SECRET_JWT_SEED=Esto-Es-UnA-Palbr@_SecretA
        ```

## Uso

1. Inicia el servidor:
    ```sh
    npm start
    ```

## Endpoints

### Autenticación

- `POST /api/auth/new`: Crear un nuevo usuario.
- `POST /api/auth`: Iniciar sesión.
- `GET /api/auth/renew`: Renovar token.

### Eventos

- `GET /api/events`: Obtener todos los eventos.
- `POST /api/events`: Crear un nuevo evento.
- `PUT /api/events/:id`: Actualizar un evento existente.
- `DELETE /api/events/:id`: Eliminar un evento.


## Librerías Utilizadas

- [Express](https://expressjs.com/): Framework de Node.js para construir aplicaciones web.
- [Mongoose](https://mongoosejs.com/): ODM para MongoDB.
- [Express Validator](https://express-validator.github.io/docs/): Middleware para validación de datos.
- [jsonwebtoken](https://github.com/auth0/node-jsonwebtoken): Implementación de JSON Web Tokens.
- [bcryptjs](https://github.com/dcodeIO/bcrypt.js): Biblioteca para encriptar contraseñas.
- [dotenv](https://github.com/motdotla/dotenv): Cargar variables de entorno desde un archivo `.env`.
- [cors](https://github.com/expressjs/cors): Middleware para habilitar CORS (Cross-Origin Resource Sharing).
- [nodemon](https://github.com/remy/nodemon): Herramienta que ayuda a desarrollar aplicaciones basadas en Node.js reiniciando automáticamente la aplicación cuando se detectan cambios en los archivos.