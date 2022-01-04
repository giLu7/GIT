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

Fast-fodward - unión automática (no hay ningun cambio que se solape con lo que está en la otra rama)

Recursiva - uniones automáticas (no hay colisiones de cambios)

Manual - tiene conflictos (ocurre cuando hay modificaciones en las mismas lineas)
