# Practica1Softca

Comandos utilizados en el ejercicio practico de Git

57302@LAPTOP-INMK8P3O MINGW64 ~/Desktop/Git y GitHub
    $ git clone git@github.com:JuanGuerra02/Practica1Softca.git
        Clonomos el repositorio a nuestra carpeta de proyectos


57302@LAPTOP-INMK8P3O MINGW64 ~/Desktop/Git y GitHub
    $ cd Practica1Softca/
        accedemos a la carpeta del repositorio clonado eh insertamos datos en README.MD


57302@LAPTOP-INMK8P3O MINGW64 ~/Desktop/Git y GitHub/Practica1Softca (main)
    $ git status
        Observamos el estado del archivo modificado     (modified: README.md)

$ git add README.md
    Se agregan los cambios a Staging

$ git commit -m "commit inicial"
    Se envian los cambios al repositorio local

$ git push origin main
    Enviamos los cambios al repositorio remoto

$ touch privado.txt
    creamos el archivo privado.txt

$ mkdir privada
    Creamos la carpeta privada

Se crea el archivo .gitignore y se agrega lo que se quiere ignorar (/privada, privado.txt)

$ touch 1.txt
    Se crea el archivo 1.txt

$ git add .
$ git commit -m "añadiendo ficheros al repositorio local"

$ git tag -a v0.1 -m "Primer avance de ejercicio practico" 49d88f7
    Se creea el tag v0.1

$ git pull origin main
$ git push origin --tags
    Se sube el tag al repositorio remoto

$ git branch v0.2
$ git checkout v0.2
    Creamos la rama "v0.2" y nos ubicamos en la rama "v0.2"

$ git push origin v0.2
    Subimos rama al repositorio remoto

$ git checkout main
$ git pull origin master
$ git merge v.02
    Nos ubicamos en la rama "main", y hacemos el merch de la rama v0.2 en la rama main

$ git commit -am "Se agrega Hola en el fichero 1.txt"
$ git checkout v0.2
$ git commit -am "Se agrega Adios en el fichero 1.txt"
$ git checkout main
$ git merge v0.2
$ git commit -am "Se aceptan ambos cambios, conflicto solucionado"
    [main 08a5e94] Se aceptan ambos cambios, conflicto solucionado

$ git branch --merged
* main
  v0.2
    Nos muestra 2 ramas con merge

$ git branch --no-merged
    No nos muestra ramas sin merge (todas estan involucradas)

$ git tag -a v0.2 -m "Segundo avance de ejercicio practico" 08a5e94
