# Comandos Git

lista los archivos se tienen para hacerles seguimiento

    git status

agrega los archivos a hacer seguimientos de futuros cambios

    git add <DIR>

agrega todos los archivos a hacer seguimiento

    git add .

se eetiqueta con un nombre el cambio a la archivo recien agregado o actualizado

    git commit -m "AQUI VA TU MENSAJE"

# comandos para moverse dentro de git

deja de hacer seguimiento a los archivos e elimina los commits se puede decir que lo hace de manaera suave

    git reset --mixed <ID-COMMIT> (default)

deja de hacer seguimiento y elimina los archivos

    git reset --hard <ID-COMMIT>

permite ver el historial de acciones realizadas con una breve descripcion de los commits

    git reflog

permite revisar los cambios de un commit en especifico. importante no realizar ningun cambio ya que generara un conflicto

tambien se puede usar para cambiar entre la rama a trabajar a las que esten disponibles

    git checkout <ID-COMMIT> / <NAME-BRANCH>

# Comandos Github

permite enlazar con eel repositorio remoto

    git remote add origin <URL_REPOSITORY>

permite revisar que url remota esta enlazada

    git remote -v

permite subir los cambios previamente se tengan los commits hechos es decir se hayan cumplido los pasos

    git add
    git commit -m "This commit"

luego de ello entraria el nuevo comando

    git push -u

si se quieren traer los cambios que esten disponibles

    git pull

# comando adicionales

es recomendable utilizarlo cuando tenemos
enlazada un repositorio remoto. este comanod se encarga de borrar un commit especifico y crea uno buevo

    git revert <ID-COMMII>

utilizado para crear nuevas ramas

    git branch <NAME>

y como habiamos visto usamos que?

    git checkout <NAME-BRANCH>

exacto usamos git checkout para revisar la nueva rama
claro que tmb podemos usar un switch

    git switch <NAME-BRANCH>

sirvee para fusionar las ramas importante .
se debe estar en la rama a la cual se quiere fusionar y que conserve los cambios y de haber cambiado dentro de la misma rama un diferentes archivos se genera un conflicto

    git merge <OTHER-BRANCH>

utilizamos los tag para decir epa hasta aca mi primera version del proyecto o la aplicacion

    git tag <NAME-TAG> -m "VERSION-NUMBER"

para subir los tag al repositorio remoto se usa

    git push --tags
