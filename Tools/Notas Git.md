﻿git init

git add index.html

git add .

git commit -m "Mensaje"

git push

git log --oneline < Muestra los commits

git reset --hard [commit] < Viajamos a cierto commit

git remote -v < Chequeamos la conexion remota a la nube que tenemos enlazada a nuestro repo local

git pull < trae archivos del ultimo commit

git fetch < Hace una comparacion del repo local y repo de la nube y los iguala

Tag

git tag [nombre tag] -m Descripcion de version" < Se hace el tag sobre el commit que estamos, navegamos entre los commit con reset y les vamos asignando distintos tags

git push --tags < Subir tags a github

Branchs

git branch < Nos muestra las ramas que hay y en la que estamos

git branch [Nombre branch] < Creamos la rama pero no nos movemos a ella

git checkout [Nombre branch] < Nos movemos a la rama

Si sobre la rama hacemos un add . y un commit -m ... se graba todo en la rama que estamos, nos tenemos que despues mover a la rama

master o main con checkout y vamos a hacer un merge

git merge [Nombre branch a unir] < Ya ubicados en el master o main tenemos que hacer que la rama que se modifico antes se una al main

git branch -d [Nombre branch] < Eliminar la rama

Si se hace un merge entre 2 ramas con conflictos que se modifico la misma parte en distintas branches vs nos va a preguntar con cual querdarnos, despues de solucionar todo hacemos un add ., un commit y un push.

Para hacer un push de la rama hay que hacer desde la rama:

git add .

git commit -m "Mensajito"

git push (Nombre de repositorio de gitHub que casi siempre es origin) (Nombre de la rama)

Ej: git push origin ramaIvan

Desde el repositorio en la nube se ve si el commit se puede hacer merge o no con el main en la nube
