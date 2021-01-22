## Comandos útiles de GIT
```ruby 
1.  git init
2.  git add .
        - git add _nombre fichero p.e index.html_ - \*añade los cambios efectuados en este fichero\*
        - git add . or git add --all - \*añade todos los cambios efectuados hasta el momento\*
3.  git commit -m "texto" - \*explicación de los cambios\*
        - git commit --amend - \*para modificar el texto de los cambios hechos anteriormente en la escritura de commits\*
        - git commit -am - \*junta git add . + git commit -m. Sólo en casos de seguimientos continuos\*
4.  git checkout -- . - \*para coger la información del último commit guardado en caso de error. Vuelta atrà de un commit\*
5.  git log
6.  git checkout -b _nombreRama_ - \*nueva rama\*
7.  checkout master/main - \*cambio de una rama a otra p.e. rama-heroes a main\*
8.  git branch -d _nombreRama_ - \*para borrar una rama que ya no utilizamos\*
9.  git push
10. 
```
## Cómo cambiar la URL remota en GIT 

. git remote set-url origin https://github.org/repo.git - \*para poder hacer los push correctamente\*

# consultas de GIT

1. ls -al - \*nos enseña todo lo que hay en la carpeta\*
2. git log --oneline --decorate --all --graph - \*nos enseña todas las relaciones del fichero y en que situación se encuentran\*
3. git status -s - \*otra forma de enseñarnos el status. En lugar de colorear nos pone letras de las acciones realizadas\*
4. 
5. 
6. 

## Formas de borrar
1. git reset *_nombre de la extensión p.e .xml_ - \*para borar ficheros del stage o cualquier  otra cosa\*
2. git reset .

## push
*git push -f origin main - para forzar un push




