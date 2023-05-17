# Como resolver un conflicto cuando el remoto es distinto al local

## Estado inicial

Tenemos el repositorio local y remoto sincronizado.

## Cambios

Una persona hace cambios en el remoto, y yo hago cambios en mi repositorio local en las mismas lineas.

## Toca resolver cambios en el local

Debo tener mis cambios en local commiteados.

```{Bash}
git add .
git commit -m "cambios importantes en las mismas lineas que el repo remoto"
```

El problema esta cuando al querer hacer un push, no podremos porque el repo local y el repo remoto no están sincronizados.

```{Bash}
git pull remote orign # ( no funcionara)
```

Lo primero es verificar si estamos en la rama correcta con git branch.

```{Bash}
git branch
```

Si estamos en la correcta, podemos proseguir, si no debemos cambiar a la rama correcta

```{Bash}
git checkout <nombre de la rama correcta>
```

Entonces lo que tendremos que hacer será hacer un rebase.

```{Bash}
git pull --rebase
```

Resolveremos los conflictos en visual estudio code, seleccionando lo que nos sirve y lo que no.

Luego procedemos a agregar los cambios con un git add

```{Bash}
git add .
git commit -m <nombre del commit>
```

Una vez hecho esto podemos decirle a git que arreglamos el conflicto con un rebase.

```{Bash}
git rebase --continue
```

Una vez tenemos todo en orden, podemos subir nuestros cambios al repositorio remoto.

```{Bash}
git pull origin main
```
