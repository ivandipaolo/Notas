﻿1- Importamos en el componente que querramos evaluar los tipos de los props lo siguiente:

import PropTypes from 'prop-types';

2- En el final del final de la funcion del componente, antes del export default (cuando tengamos) ponemos

NombreComponente.propTypes = {

}

3- Estos PropTypes:

https://es.reactjs.org/docs/typechecking-with-proptypes.html
