﻿
//Se concatena el endpoint del url en el primer param

fetch(url + 'login', {

method: 'POST',// Se expecifica metodo que se va a usar

body: JSON.stringify(formData), // Se serealiza la data de la peticion

headers: {'Content-Type': 'application/json'} //Decirle al backend que es un tipo json

})//Es una promesa

.then(resp => resp.json()) //Pedimos que pase la response del back a json

.then(data => {

console.log(data)

})//Pedimos que imprima la data

.catch(err => console.log(err)) //Si hay error pedimos q lo imprima con catch

en el segundo .then se puede hacer

.then(({msg, token}) => { // Desestructuramos esto del objeto

if(msg){

return console.error(msg)

}

localStorage.setItem("token", token)

})
