﻿1- Crear el archivo.js del custom hook en la carpeta hooks en el src anteponiendo use...

2- export const useCustomHook = (initialState = 10) => {}

No pasa de ser una funcion de flecha con un return que lo mejor es que sea objeto para desestructurar despues lo que querramos usar...

Puede ser un array tmb el return.

3- Puede recibir parametros como en el ejemplo, puede usar useState y useEffect.

4- En el caso que tengamos lo siguiente para modificar un estado del custom hook:

const increment = (num = 1) => {

setstate(state + num)

}

ya en el lugar donde usemos el hook no se puede poner onClick={increment} porque toma como que se esta pasando el evento como parametro y tira cualquier cosa, se empieza a hacer onClick={() => increment()}

5- Cuando se desestructura un custom hook en el componente que lo usemos se le puede pasar parametros ej:

Objeto:

const {ej1, ej2} = useCustomHook('Hola Mundo');

Osea en vez de tener:

const [value, setValue] = useState(asd)

se hace una desestructuracion del custom hook que devuelve un array y queda:

const [value, funcionDelHook] = useCustomHook(asd)
