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

### Subir una etiqueta (tag) en especifico

```sh
git push origin <tag_name>
```

### Subir todos tags (NO RECOMENDADO)

```sh
git push --tags
```

### Borrar tags

```sh
git tag -d <tag_name>
```

### Git Amend

Sirve para cuando uno se equivoca sobre en el último commit. Por ejemplo al hacer un commit y olvidarse de guardar el archivo que estaba modificando

```sh
git commmit --amend
```

Recuerden que no solo pueden cambiar el nombre del commit también pueden agregar archivos.

### Guía buenas prácticas para nombrar a los commits

https://medium.com/@jmz12/buenas-pr%C3%A1cticas-para-commits-5eb4c86b9a47

### IMPORTANTE: USAR CON CUIDADO

```sh
git checkout -- .
```

# GIT RESET

```sh
git reset --soft
```

```sh
git reset === git reset --mixed
```

Es más destructivo de todos.

```sh
git reset --hard
```

# GIT REFLOG

Nos muestra la historia completa incluido todos los movimientos que fuimos haciendo sobre nuestro
repositorio.

```sh
git reflog
```

Vuelvo al punto donde quiero estar, colocando el hash en checkout.

```sh
git checkout <HASH> .
```

# REBASE

¿Cómo actualizo una rama de v con los cambios en master antes de integrar los cambios que tienen la rama dev?

git rebase master > crea un area temporal, mueve los commits de la rama dev y mueve al al último commit y luego mueve los commits del area temporal al final de los commits

### Rebase interactivo

```sh
git rebase -i <HASH>
```

Ej:

git rebase master > crea un area temporal, mueve los commits de la rama dev y mueve al al último commit y luego mueve los commits del area temporal al final de los commits

```sh
git rebase -i 8fee621
```
