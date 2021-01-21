#Comandos útiles de GIT

1. git init
2. git add .
3. git reset .
4. git commit
5. git checkout -- . (per agafar la informació del ultim commit guardat en cas d'un error)
6. git log
7. git commit --amend (per a modificar detalls d'escritura dels commits)
8. git checkout -b rama-heroes (nova branca)
9. checkout master/main (canvi d'una branca a una altra. p.e. rama-heroes a main)
10. git branch -d rama-heroes (per borrar una branca que ja no utilitzem)
11. git push
12. git commit -am (junta git add . + git commit -m. Només en casos en seguiments continuos)

# Cómo cambiar la URL remota en GIT 

. git remote set-url origin https://github.org/repo.git - para poder hacer los push correctamente

# consultas de GIT

.git add (nombre fichero p.e index.html) - añade los cambios efectuados en este fichero
.git add . or .git add --all - añade todos los cambios efectuados hasta el momento
.ls -al - nos enseña todo lo que hay en la carpeta
.git reset *(nombre de la extensión p.e. .xml) para borar ficheros del stage o cualquier  otra cosa
.git log --onelin --decorate --all --graph - nos enseña todas las relaciones del fichero y en que situación se encuentran
.git status -s - otra forma de enseñarnos el status. En lugar de colorear nos pone letras de las acciones realizadas

# push
.git push -f origin main - para forzar un push




