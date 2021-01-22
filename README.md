https://docs.github.com/es/github/writing-on-github/getting-started-with-writing-and-formatting-on-github
## Comando iniciales##

* git config --global user.name _(nombre de quien va a hacer el código)_
* git config --global user.email _(email de quien va a hacer el código)_

## Comandos de GIT##
```ruby 
1.  git init - \*crea una carpeta .git y una rama main/master\*
        - git clone URL - \*baja el repertorio de GITHUB que queremos trabajar a local\*
        - git remote add origin URL - \*enlaza repertori local con repertorio en la nube vacio\*
2.  git add .
        - git add _nombre fichero p.e index.html_ - \*guarda los cambios efectuados en este fichero. Podemos ecoger que queremos guardar\*
        - git add . or git add --all - \*guarda todos los cambios efectuados hasta el momento\*
3.  git commit -m "texto" - \*Registra los cambios con una explicación de los cambios\*
        - git commit --amend - \*para modificar el texto de los cambios hechos anteriormente en la escritura de commits\*
        - git commit -am - \*junta git add . + git commit -m. Sólo en casos de seguimientos continuos\*
4.  git checkout -- . - \*para coger la información del último commit guardado en caso de error. Vuelta atrà de un commit\*
5.  git log - \*nos enseña toda la información\*
        - git log --oneline - \*nos enseña la información de los cambios pero sólo una línea\*
6.  git checkout -b _nombreRama_ - \*crear nueva rama\*
7.  git checkout master/main - \*cambio de una rama a otra p.e. rama-heroes a main\*
8.  git merge _nombreRamaAuxiliar_ - \*tenemos que estar dentro de la rama principal main/master y le indicamos que rama queremos incluir la información en la
                                        rama principal\*
9.  git branch -d _nombreRama_ - \*para borrar una rama que ya no utilizamos\*
10. git push
 
```
## Cómo cambiar la URL remota en GIT##

. git remote set-url origin https://github.org/repo.git - < para poder hacer los push correctamente >

# consultas de GIT##

1. ls -al - \*nos enseña todo lo que hay en la carpeta\*
2. git log --oneline --decorate --all --graph - \*nos enseña todas las relaciones del fichero y en que situación se encuentran\*
3. git status - \*Indica en rojo los archivos con cambios\*
        - git status -s - \*otra forma de enseñarnos el status. En lugar de colorear nos pone letras de las acciones realizadas\*
4. git log -g - \*aparecen commits perdidos\*
5. git remote -v - nos enseña la url de GITHUB de la carpeta de destino
6. 

## Formas de borrar##
1. git reset *_nombre de la extensión p.e .xml_ - \*para borrar ficheros del stage o cualquier otra cosa\*
2. git reset .
3. git gc - \*garbage collector. recolector de basura. Para borrar definitivamente no tiene que haber nada en branch, tag y reflog\*

## push##
*git push -f origin main - para forzar un push




