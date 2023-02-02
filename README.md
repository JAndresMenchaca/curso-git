# Curso Git

```python
pwd  # ver directorio de trabajo

git init # iniciar un repositorio

git status # ver el estado de los archivos

git add index.html # añadir un archivo al repositorio

git commit -m "Add index.html" # subir una nueva version del codigo

git checkout f4e01 # volver a una version anterior

git checkout master # volver a la ultima version

git reset f4e01 # sobreescribir los cambios en un commit ya creado

git reset --hard c255fb # si queremos borrar todos los cambios que hicimos despues de hacer el commit, vuelve a la version original de esa version.
			Si lo aplicamos en una version que no es el master, el commit se borra por completo.

git log --oneline # muestra los commits pero en una sola linea

rm index.html # Borrar el archivo

git restore index.html # recuperar el archivo, si ya existe lo pone en la version original

git add . # añadir todas los archivos de ese directorio

git remote add origin git@github.com:JAndresMenchaca/curso-git.git # establecer el origen del servidor remoto, para subir el proyecto al repositorio de Github

git remote -v # para ver el origen

pass # sotwa195anders

git push origin MASTER # poner la rama que queremos subir, si ponemos -u antes de origin se crea la nueva rama y se sube todo

git clone git@github.com:JAndresMenchaca/curso-git.git # descargar repositorio
ORDEN:

1. git status
2. git add .
3. git commit -m "Change div"
4. git push


git checkout  -b feature-post-styles # se utiliza para cambiar o crear una rama

git branch # nos muestra la rama en la que estamos, y las ramas disponibles. Si la creamos desde una rama secundaria, se crea a partir de esa rama

git push -u origin feature-post-styles # crear rama en GitHub

git checkout master # volver a la rama de master

git pull # fusionar las ramas de forma local

git merge _nombre_rama_ # fusionar dos ramas en local. Antes, en la rama secundaria debemos hacer un add, commit. Y luego en la rama donde queremos los cambios hacemos merge

git log --graph --oneline

git remote -v # ver el origin

git commit -a -m "Cambio backend 2" # atajo para ya no hacer git add .

git log -n 3 # pedir un numero especifico de los ultimos commits

git log --graph # con gragico


Si hicieramos el rebase estando en feature-affiliate-links y trayendo front, no haría falta hacer el merge del final. Es decir:

git checkout feature-affiliate-links
git rebase -i *nombre_rama*
Al hacer un merge o rebase es mejor pensarlo como "qué rama me quiero traer aquí?" en lugar de "dónde me quiero llevar esta rama?"

git branch -d *nombre_rama* # borra una rama

git branch -D *nombre_rama* # la borra sin importarle nada

git commit --amend -m "cambio video 3" # sirve para reemplazar la descripcion del ultimo commit

git stash # deshacer los cambios sin perderlos
git stash pop # volver a tener lo que borramos

versionado semantico

git tag -a v0.1.0 -m "Primera version" # es para poner versiones a los commits
git tag # listado de tags
git show v0.1.0 # nos muestra los detalles de la version 
git push origin v0.1.0 # lo lleva a GitHub

.gitignore
```

Curso Git Mastermind