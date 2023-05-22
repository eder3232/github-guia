# Comandos relacionados con el stage

## Agregar archivo

```{Bash}
git add index.html
```

## Agregar todos los archivos html del root

```{Bash}
git add *.html
```

## Quitar archivo del stage

```{Bash}
git reset index.html
```

## Agregar commit

```{Bash}
git commit -m <nombre del commit>
```

## Regresar el repo a como estaba el último commit

```{Bash}
git checkout -- .
```

## Seguimiento de carpetas vacias

Cuando se tiene una carpeta vacia y se le quiere dar seguimiento, se debe crear un archivo llamado .gitkeep, porque de lo contrario, git no hace seguimiento de carpetas vacias, esto podria ser el caso de una carpeta vacia llamada uploads.

## Ver el estado simplificado

```{Bash}
git status --short
```

## Ver los cambios

```{Bash}
git diff
```

## Ver los cambios en el stage

No se recomienda usar

```{Bash}
git diff --staged
```
