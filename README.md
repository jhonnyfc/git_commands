# git_commands

### Crear una nueva rama

```
$ git checkout -b new_nam_branch
$ git branch new_branch_name
```

### Saber en que rama estamos

```
$ git branch -a
```

### Cambiar a otra rama

```
$ git checkout branch_name
$ git switch branch_name
```

### Subir la branch a el servidor

```
$ git push origin branch_name
```

### Hacer un push forzado y sin pasar test, linter si esta activado

```
$ git push --force-with-lease --no-verify
```

### Ver las ramas

```
$ git log --graph
```

### Los ultimos 20 log de todas las ramas

```
$ git log --graph --oneline --all -20
```

### Unir dos ramas, situarse en la rama general y luego hacer merge

```
$ git merge rama_a_traer
```

### Abortat merge

```
  $ git merge --abort
```

### Recuperar aricho borrado con git

First you need to reset the status of abc.c in the index:

    $ git reset -- abc.c

Then you need to restore abc.c in your working tree:

    $ git checkout -- abc.c

### Deshacer todos los cambios que aun no estan staged

```
  $ git checkout .
```

### Deshacer X commits realizados desde el HEAD

```
  $ git reset HEAD~X
```

### Hace un rebase interactivo con los X commits desde el Head

```
  $ git rebase -i HEAD~X
```

### Mostar configuracion actual de git

```
  $ git config -l
```

### Cambiar de gitlab a github:

Quitar el origin de gitLab y poner el de git hub y luego pushear, <br> pude que tengas que añadir tu clave ssh publica a github.

    $ git remote remove origin
    $ git remote add origin git@github.com:USERNAME/REPO_NAME.git
    $ git push origin master

### SSH link and HTTP link construction

```
	https://github.com/jhonnyfc/git_commands.git
```

```
	git@github.com:jhonnyfc/git_commands.git
```
