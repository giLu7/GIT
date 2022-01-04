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
