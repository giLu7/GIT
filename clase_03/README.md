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

# Fork

Me permite crear un repo en mi cuenta de cualquier proyecto de Github

1. Vamos al repo que queremos hacer el fork. Presionamos el botón.
2. Se crea el repo en mi cuenta.
3. Puedo clonar ese repo y empezar a trabajar
