# Clase 02 - GIT

## GIT LOG

### Muestra los commits

```sh
git log
```

**NOTA:** Para salir es con la letra **q**

### Muestra los commits en forma abreviada

```sh
git log --oneline
```

### Por fecha

```sh
git log --since="2021-12-20"
git log --after="2021-12-20"
git log --before="2021-12-27"
git log --after="2021-12-20" --before="2021-12-27"
```

### Muestra la cantidad de commits elegidos.

Ejemplo: 2 commits

```sh
git log -2 # cantidad de commits que va a mostrar el git log
```

```sh
git log --oneline --decorate --all --graph
```

GIT IGNORE
Sirve para ignorar archivos que no quiero seguir.

Creo el archivo **.gitignore** en el directorio raíz y dentro coloco el nombre del arhivo o la carpeta que no quiero seguir.

### GIT KEEP

Me permite seguir una carpeta vacía

Creo un archivo llamado **.gitkeep** que lo que hace es tener en cuenta la carpeta vacía

## IMPORTANTE: Forma corta de hacer un git add y un git commit

NOTA: Tengo que tener todos los archivos seguidos. Si tengo un archivo untracked ese archivo no se va a commitear

```sh
git commit -am "mensaje commit"
```

## REMOTE

#### Lista alias de remotos

```sh
git remote -v
```

#### Lista alias de remotos y urls

```sh
git remote -v
```

#### Agrego remoto a mi REPO

```sh
git remote....
```

#### Renombra el alias de la URL del remoto

```sh
git remote rename <nombre-antiguo> <nombre-nuevo>
```

### Forma corta de hacer un status y ver los cambios en el working directory

```sh
git status --short
```
