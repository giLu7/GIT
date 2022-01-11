# Clase 04

## Git Gist

Permite crear pequeños snippets de código para compartir.

## GitPages

En los settings del proyecto, en el sidebar buscamos Pages y ahí habilitamos para que el repo se empiece a servir en la web

## Git Tag

### Tag en el último commit

```sh
git tag -a v1.0.0 -m "Versión 1.0.0"
```

### Tag en un commit en especifico

```sh
git tag -a v1.0.0 <HASH> -m "Versión 1.0.0"
```

### Listar todos los tags

```sh
git tag
```

### Más información de un tag en particular

```sh
git show <indentificadorDelTag>
```

Ejemplo:

```sh
git show v1.0.0
```

### Tag en el ultimo commit

```sh
git show <identificador del tag>
```
