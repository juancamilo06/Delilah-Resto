# Delilah Resto
![page-1-admin1](https://user-images.githubusercontent.com/71902702/129285541-ae7f2ce2-9374-44ea-b503-2a9357113fa6.png)

Proyecto Delilah-Resto del curso de Desarrollo Web Full Stack de Acamica.

El proyecto consistió en crear el BackEnd de una API que le permita a los usuarios registrarse, ver un listado de productos disponibles y realizar pedidos de los mismos a un restaurant.
Para realizar dicha tarea la API consume y genera información en una base de datos relacional (mySQL) mediante distintos endpoints establecidos.

## Funcionalidades del proyecto

- Crear un usuario.
- Autenticación de un usuario ya registrado.
- Busqueda de usuarios `(general o por id)`.
- Cambio de permisos de un usuario `(solo por un admin)`.
- Deshabilitación de un usuario `(solo por un admin)`.
- Busqueda de productos `(general o por id)`.
- Cambio de parametros de un producto `(solo por un admin)`.
- Desabilitación de un producto `(solo por un admin)`.
- Busqueda de pedidos `(general o por id)`.
- Cambio del estado de un pedido `(solo por un admin)`.
- Cancelación de un pedido `(solo por un admin)`.

## Recursos y tecnologías utilizadas

- Node
- ExpressJs
- Sequelize
- MySQL
- JWT
- Dotenv
- Postman

## Como instalar y utilizar la API

### 1 - Clonar proyecto

Clonar el repositorio 
Desde la consola con el siguiente link:
`git clone https://github.com/juancamilo06/Delilah-Resto-Acamica.git .`

### 2 - Instalación de dependencias

```
npm install
```

### 3 - Crear e importa la Base de datos

- Abrir con XAMPP u otro programa alternativo que soporte MySQL un servidor local y asegurarse que el puerto sobre el cual se está ejecutando es el `3306`
- Inicializar los servicios de Apache y MySQL
- Abrir el panel de control del servicio MySQL
- Generar una nueva base de datos llamada `delilah`.
- Dentro del `panel de control` de la base de datos creada importar el archivo `/db/database.sql`.

### 4 - Iniciar el servidor

- Crear un archivo `.env` en el repositorio local y declararle las siguientes variables.

```
DB_CONNECT = mysql://root:@localhost:3306/delilah
TOKEN_SECRET = jwtpass
```

- En la consola del IDE correr el comando `npm run start` o `npm run dev` recomiendo entrar directamente a la documentacion y testear desde postman.

### 5 - Ya lo puedes usar!

Testear los endpoints provistos desde postman para poder hacer uso de la API y base de datos generadas

## Documentación de la API

### [Postman - Delilah API v1](https://documenter.getpostman.com/view/11682039/TVCjx5su)
