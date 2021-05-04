## [Start GIT - Resume](https://docs.github.com/es/github/writing-on-github/getting-started-with-writing-and-formatting-on-github)
Es una buena idea mantener todas las carpetas del repositorio local dentro de una carpeta principal del equipo. Esto mantiene su trabajo de Git muy bien organizado.
## Resume: Pasos a seguir:
<ul>
	<li>Identify benefits of using Git</li>
	<li>Describe a repository</li>
	<li>Describe a commit</li>
	<li>Create a local repository</li>
	<li>Commit to a local repository</li>
	<li>Create a remote repository</li>
	<li>Push to a remote repository</li>
	<li>Differentiate between the working tree, staging area, local repository and remote repository</li>
</ul>

## Metodología: Inicio git
* git config --global user.name _(nombre de quien va a hacer el código)
* git config --global user.email _(email de quien va a hacer el código)
  ### Installation and Getting Started
[sourcetree_installation](https://github.com/ConxiCR/youtube-git/blob/61c182b0a38ef98787268f212a8c6f4e72ad2f43/lab3_1_02a_sourcetree_installation.pdf). Instalación de Sourcetree.

[cli_installation](https://github.com/ConxiCR/youtube-git/blob/9b223dc65b07a7a2dc8f4eae38729bd9392ed8fb/lab3_1_02b_cli_installation.pdf). Instalación de GIT con línea de comandos.
## GIT locations
 El árbol de trabajo contiene los archivos de proyecto para una sola confirmación, el área de ensayo contiene una lista de archivos que se incluirán en la siguiente confirmación, el repositorio local contiene todas las confirmaciones del proyecto. En su equipo local.
### [Create a local repository with sourcetree](https://github.com/ConxiCR/youtube-git/blob/ef2daeb333039fe5d2b2e965f9a7ee0d317f8b57/GITInstructions/lab3_1_03a_sourcetree_create_local_repository.pdf)
### [Create a local repository with CLI linea de comandos](https://github.com/ConxiCR/youtube-git/blob/be6415ceae39b132e06f78acde195f0888aac25b/GITInstructions/lab3_1_03b_cli_create_local_repositoryWithGit.pdf)
### [Create a commit with sourcetree](https://github.com/ConxiCR/youtube-git/blob/c730e2eaa06ea4d124421fde64372601f4ddd6c3/GITInstructions/lab3_1_04a_sourcetree_commit.pdf)
### [Create a commit with CLI](https://github.com/ConxiCR/youtube-git/blob/c730e2eaa06ea4d124421fde64372601f4ddd6c3/GITInstructions/lab3_1_04b_cli_commit.pdf)



<!--
    Git status -> Mirar si tienes modificaciones tuyas y si existe algún pull o push
    Git fetch -> Por si acaso tus ramas no se han actualizado correctamente, esto NO actualiza los ficheros de las ramas, sólo el estado de esa rama
    Git status -> Para verificar de nuevo modificaciones, pull y pushs
    Git pull -> Ahora sí descargas las actualizaciones
    Git add/commit/... -> Ahora guardas tus modificaciones
    Git status -> Miras que siga sin necesitar un pull, por si las moscas
    Git push -> Subes tus datos
    Git status -> Compruebas que está todo correctamente-->



## Comandos de GIT
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
### Cómo cambiar la URL remota en GIT##
. git remote set-url origin https://github.org/repo.git - < para poder hacer los push correctamente >

### Cómo eliminar una URL remota de Git
https://www.delftstack.com/es/howto/git/how-to-remove-a-git-remote-url/

### consultas de GIT
 Git log -> Para comprobar que está correctamente comiteado lo que has pusheado
 Para salir de Git log, pulsa "Q"

1. ls -al - \*nos enseña todo lo que hay en la carpeta\*
2. git log --oneline --decorate --all --graph - \*nos enseña todas las relaciones del fichero y en que situación se encuentran\*
3. git status - \*Indica en rojo los archivos con cambios\*
        - git status -s - \*otra forma de enseñarnos el status. En lugar de colorear nos pone letras de las acciones realizadas\*
4. git log -g - \*aparecen commits perdidos\*
5. git remote -v - nos enseña la url de GITHUB de la carpeta de destino

### Formas de borrar
1. git reset *_nombre de la extensión p.e .xml_ - \*para borrar ficheros del stage o cualquier otra cosa\*
2. git reset .
3. git gc - \*garbage collector. recolector de basura. Para borrar definitivamente no tiene que haber nada en branch, tag y reflog\*

### SOS push
*git push -f origin main - para forzar un push




