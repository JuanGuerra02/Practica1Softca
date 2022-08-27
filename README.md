# Practica1Softca

Comandos utilizados en el ejercicio practico de Git

57302@LAPTOP-INMK8P3O MINGW64 ~/Desktop/Git y GitHub
```ssh
$ git clone git@github.com:JuanGuerra02/Practica1Softca.git
``` 
Clonomos el repositorio a nuestra carpeta de proyectos


57302@LAPTOP-INMK8P3O MINGW64 ~/Desktop/Git y GitHub
```ssh
$ cd Practica1Softca/
```
accedemos a la carpeta del repositorio clonado eh insertamos datos en README.MD


57302@LAPTOP-INMK8P3O MINGW64 ~/Desktop/Git y GitHub/Practica1Softca (main)
```ssh
$ git status
```
Observamos el estado del archivo modificado     (modified: README.md)
```ssh
$ git add README.md
```
Se agregan los cambios a Staging
```ssh
$ git commit -m "commit inicial"
 ```
 Se envian los cambios al repositorio local
```ssh
$ git push origin main
 ```
 Enviamos los cambios al repositorio remoto
```ssh
$ touch privado.txt
 ```
 creamos el archivo privado.txt
```ssh
$ mkdir privada
 ```
 Creamos la carpeta privada

-Se crea el archivo .gitignore y se agrega lo que se quiere ignorar (/privada, privado.txt)
```ssh
$ touch 1.txt
 ```
 Se crea el archivo 1.txt
```ssh
$ git add .
$ git commit -m "añadiendo ficheros al repositorio local"
```

```ssh
$ git tag -a v0.1 -m "Primer avance de ejercicio practico" 49d88f7
```
Se creea el tag v0.1
```ssh
$ git pull origin main
$ git push origin --tags
 ```
 Se sube el tag al repositorio remoto
```ssh
$ git branch v0.2
$ git checkout v0.2
 ```
 Creamos la rama "v0.2" y nos ubicamos en la rama "v0.2"
```ssh
$ git push origin v0.2
 ```
 Subimos rama al repositorio remoto
```ssh
$ git checkout main
$ git pull origin master
$ git merge v.02
```
Nos ubicamos en la rama "main", y hacemos el merch de la rama v0.2 en la rama main
```ssh
$ git commit -am "Se agrega Hola en el fichero 1.txt"
$ git checkout v0.2
$ git commit -am "Se agrega Adios en el fichero 1.txt"
$ git checkout main
$ git merge v0.2
$ git commit -am "Se aceptan ambos cambios, conflicto solucionado"
 ```
 [main 08a5e94] Se aceptan ambos cambios, conflicto solucionado
```ssh
$ git branch --merged
```
* main
  v0.2
    Nos muestra 2 ramas con merge
```ssh
$ git branch --no-merged
 ```
 No nos muestra ramas sin merge (todas estan involucradas)
```ssh
$ git tag -a v0.2 -m "Segundo avance de ejercicio practico" 08a5e94
```
```ssh
$ git branch -d v0.2
```
Deleted branch v0.2 (was f991504).


Listar los distintos commits con sus ramas y sus tags
```ssh
$ alias arbol="git log --all --graph --decorate --oneline"
$ arbol
```
```ssh
* 1a21984 (HEAD -> main, tag: v0.2) Se actualiza la informacion de Readme.md
*   08a5e94 Se aceptan ambos cambios, conflicto solucionado
|\
| * f991504 Se agrega Adios en el fichero 1.txt
* | 74074d1 Se agrega Hola en el fichero 1.txt
|/
* a2ae622 (origin/v0.2) Actualizando informacion de README.md
* a74fa57 Archivo 2.txt creado en rama v0.2
* 49d88f7 (tag: v0.1, origin/main, origin/HEAD) actualziando informacion en README.MD
* a4342cb Añadiendo ficheros al repositorio local
* c92c91c correccion en texto
* e49b9f7 commit inicial
* 3f0a3e4 Initial commit
```
