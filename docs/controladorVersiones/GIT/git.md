---
sidebar_position: 1
---

# GIT

curso (añadir repositorio de github de mouredev) https://www.youtube.com/watch?v=3GymExBkKjE&t=11085s 

## interfaces graficas para git (GUI)

gitkraken - solo trabaja free con repositorios publicos
sourcetreeapp - publicos y privados free
git-fork -
git Desktop

## TEORIA

HEAD : donde estoy rtabajando ahora

*Ponerle permisos a mis repositorios asi no lo pueden cambiar

*En el caso que se quiera trabajar con un fihcero que no tienes permisos y lo quieres en tu repositorio usas el 'fork' es como un 'clone' pero solo quedara en tu repositorio 
no en el de la otra persona, esto te permitira usar su contenido

*Pull request o pr = contribuir con un proyecto

*Git flow *buscar como funciona esto*

### BUENAS PRACATICAS:

*los commits solo se deben hacer cuando ya el codigo esta funcional
*las ramas se deben eliminar una vez ya esten en produccion o ya no se vayan a usar
*antes de realizar cualquier accion revisar el git status, para ver como esta el proyecto en local antes de subirlo
RECORDATORIO configure mi git con ssh : id_rsa y esta en ficheros ocultos en servicios

## COMANDOS

- BASICOS
init , commit , add

git log - muestra todo lo que se ha echo a lo largo del projecto

git diff - dice que se agrego y borro del projecto

git checkout - realizar o revertir cambioas, cambiar de branch *no es buena practica para eso se usa el switch* (realmente es la descarga de los cambio, solo si estas local o tienes descargado esas cosas es que puedes moverte en esos cambios)

git reset - ,añadir 'hard' para irse al hash selecionado y apartir de ahi borrar todo lo que tenga arriba de el si tiene algo, en caso que sea el ultimo no borra si no al contrario recupera los archivos anteriores

git reflog - historico de las alteraciones

git tag tag_name - se usa para identifar parte de codigos (como por ejemplo versiones,) se tienen que escribir en minuscula_y_guion_bajo

git branch - crear nueva branch, nuevo flujo de trabajo  

git switch - cambiar de branch

git merge name_branch - combinar los cambios

git stash - guarda pero sin mostrar en git, es util cuando necesitas cambiar de branch y no puedes hacer commit porque no esta terminado el codigo. [pop, list, drop ]

git fetch - se descarga el historial sin los cambios

git pull - se descarga el historial y los cambios

git config --global alias.tree "git log --graph --decorate --all --oneline"

- AVANZADO

git revert - borra algo en el medio**

## GITHub

git remote add origin ssh del 'repositorio'
git push origin 'en que rama lo queremos subir ej:main' - sube a github el repositorio
