# "Delilah Restó"pedidos de comida

Trabajo #3 del curso de Desarrollo Web Full Stack de Acámica.

## Recursos y tecnologías utilizadas

- Node.js
- Express
- JWT para autenticación via Token
- MySQL
- Postman para manejo de endpoints y testing
- Swagger para documentación de API

El objetivo del trabajo es generar el backend de una app de pedidos de comida, generando la arquitectura, bases de datos relacionales, endpoints funcionales y documentación.

## Documentación de la API

Abrir el archivo `api-docs.yaml` y copiar su contenido en [Swagger](https://editor.swagger.io/) o importar el mismo desde las opciones

Se listarán los endpoints y métodos disponibles y la información necesaria para hacer uso de los mismos

## Instalación e inicializacion del proyecto

### 1 - Clonar proyecto



Descargar [Node.js](https://nodejs.org/en/) e instalarlo


Descargar [XAMPP](https://www.apachefriends.org/es/index.html) e instalar los servicios Apache y MySQL

Clonar el repositorio desde https://github.com/mabhyHs/appDelilah.

### 2 - Instalación de dependencias

```
npm install ó sudo apt install npm (en caso de linux)
```
### 3 - Creando base de datos

- Abrir XAMPP y asegurarse que el puerto sobre el cual se está ejecutando es el `3306`
- Inicializar los servicios de Apache y MySQL
- Abrir el panel de control del servicio MySQL
- Generar una nueva base de datos llamada `delilah_resto` desde el panel de control
- Abrir el archivo en `/database/queries.sql` y dentro del `panel de control` de la base de datos ejecutar la serie de queries del archivo o importar el mismo.

### 4 - Iniciando el servidor

Abrir el archivo en `/server/server.js` desde node

`node server`

### 5 - Listo para usar!

Testear los endpoints provistos desde postman para poder hacer uso de la API y base de datos generadas

Utilizar el siguiente botón [![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/8415d1cf125e836b33b0) para acceder a la colección.

En caso de error con el botón importar el archivo `Delilah.postman_collection.json` directo desde la aplicación.

Para poder hacer uso de las funcionalidades de automatización generar una variable global llamada token que es utilizada por los endpoints para poder reemplazar el token de forma dinámica.
Pasos de uso
Si el token actual no es válido, utilizar alguno de los 2 endpoints de Login, Admin o Not Admin, ambos devolverán un token con roles distintos que permitirán acceder o no a distintos endpoints.
Para testear únicamente la validez de un Token, utilizar el endpoint TEST - Validate Token

