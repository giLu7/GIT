# CLASE 03 - GIT

## Repaso de Branch

### Listo ramas

```sh
git branch
```

### Creo una rama

```sh
git branch <nombreRama>
```

### Cambio entre ramas

```sh
git switch <nombreRama>
```

### Subir rama local al remoto

```sh
git push origin <nombreRama>
```

Ej:

```sh
git push origin clase03
```

## Git Merge

### Tipos de Merge

Fast-fodward (no hay ningun cambio que se solape con lo que está en la otra rama)

Agrego cosas que quiero tener en consideración

- Tener en cuenta subir una rama al remoto
- Ver clone
- Ver fork

### Abortar Merge

```sh
git merge --abort
```

## ALIAS

### ¿Cómo creo un alias?

git config alias.lg "log --oneline --decorate --all --graph"
git config alias.l "log --oneline"

### Para editar el archivo de configuracion de GIT

```sh
git config -e
```

### Para eliminar un alias

```sh
git config --unset alias.(nombre)
```

# Git Clone

Me permite clonar cualquier repositorio que exista en GitHub, GitLab, etc.

#### Lo clona en la carpeta con el mismo nombre

```sh
git clone https://...
```

#### Clona en una carpeta en específico

```sh
git clone https://..... ./<nombreCarpeta>
```

# GIT PULL

Trae todos los cambios que hubieran surgido durante el día (por ej)

```sh
git pull

```

# Fork

Me permite crear un repo en mi cuenta de cualquier proyecto de Github

1. Vamos al repo que queremos hacer el fork. Presionamos el botón.
2. Se crea el repo en mi cuenta.
3. Puedo clonar ese repo y empezar a trabajar

# Para actualizar un Fork

Necesito el remoto original. Del remoto del repo al cual le hice el fork

## Agrego el remoto del repositorio original

```sh
git remote add upstream <urlRemotoOriginal>
```

## Me traigo los últimos commit de el repo original

```sh
git pull upstream <urlRemotoOriginal>
```

# GIT STASH

Es una pila de almacenamiento que provee GIT. Permite registrar temporalmente los cambios del working directory para seguir trabajando. Cuando hacemos un stash. Cuando hacemos un stash se reestablece el proyecto al último commit

## Crea el stash

GUarda los cambios que estan en el working directory en un área temporal

```sh
git stash
```

## Para listar los stash

```sh
git stash list
```

## Para recuperar el stash

Lo que hace este comando es recuperar el último stash

```sh
git stash pop
```

## Para cargar un stash en particular

```sh
git stash apply  stash@{0}
```

## Para borrar el stash

```sh
git stash drop stash@{0}
```
