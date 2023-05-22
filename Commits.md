# Commits

## Arreglando un commit

Si el caso es que escribiste mal el último commit se puede arreglar con:

```bash
git commit --ammend -m <mensaje corregido> 
```

## Faltaron aniadir cambios al último commit

El head apunta al último commit en la rama main.
El ^ indica el último commit antes del head.
El head se puede remplazar con el hash del commit.

``` bash
git reset --soft HEAD^
```
