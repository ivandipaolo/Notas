﻿1- Creamos la carpeta donde vamos a hacer el proyecto

2- Usamos npm init -y para el package y desp npm i

3- Creamos la carpeta models e importamos el server.js

4- Creamos el app.js y llamamos: const Server = require('./models/server');

5- Como lo que estamos llamando del modelo es una clase hacemos:

6- const server = new Server; y despues server.listen(puerto) que es el metodo para leer el puerto dentro de

la clase Server, lee el puerto del require('dotenv').config() <<< se hace arriba de todo del app.js

7- Hacemos el install de todos los packages q queremos usar

8- Creamos la carpeta public y el index.html dentro
