﻿1-Vos primero creas la ruta, con los imports del Router de express, el check de express-validator, el middleware para validar los checks q hicimos y se declara router = Router();

2-Despues definis la ruta en el servidor, en la parte de paths y la llamamos en la parte de routes con this.app.use....

3-Ponemos los mÃ©todos respectivos en el js de la ruta nueva como por ej route.get('/', (req,res) =>{res.json....})

4-Definimos los metodos de cada uno necesarios segun se soliciten en el servicio con ids o rutas necesarias

5-Creamos cada metodo en postman en carpetas para probarlos (opt)

6-Creamos coleccion en Mongo en minuscula

7-Creamos el modelo que debemos usar, se puede copiar uno ya creado si es parecido

8-Definimos el schema del modelo

9-Agregamos el modelo creado al index en models para centralizar las cosas.

10- Empezamos con cada uno de los metodos de la colleccion y sus middlewares.

11- Hacemos los checks necesarios para cada metodo

12- Se crea en la carpeta de controladores el controlador de esta ruta con el mismo nombre del js de route y adentro

vamos a definir las funciones que se van a ejecutar en esta ruta. Cada funcion es para cada metodo de la ruta.

13- En el controlador, usamos como parametros el req y el res = response, el req siempre extraemos los que se le paso por postman

con const x = req.body.loquesea

14- Importamos el modelo del controlador del index de los models y revisamos la base de datos

15- const x = await x.findOne o lo que sea...

16- Se hace un return res.status(...).json() para frenal y retornar algo de la funcion del controlador

17- Generamos dentro de la funcion del controlador un generador de la data que queremos guardar en la bd con un

const data = {}

18- Creamos el objeto a guardar en la base de datos: ej const x = new X(data) y despues la guardamos en la base de datos en la

base de datos con un await x.save() y se guarda en la db.

19- Luego de todo en el controlador hacemos un res.status(201).json({}) como para enviar que esta todo bien hecho.

20- Volviendo a los models se puede seleccionar lo que se muestra en cada schema extrayendo lo que se guarda al momento de exportar.
