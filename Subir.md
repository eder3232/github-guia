# Como subir tu repo

## Creamos repositorio en github (web)

En este incluire el README.md y LICENSE (cambiado a main).

## Inicializamos repositorio en local

```{Bash}
git init
```

## Agregamos el repositorio remoto

```{Bash}
git remote add origin [link del repositorio remoto]
```

## Cambio el nombre de la rama local

```{Bash}
git branch -M main
```

## Hacer el pull del repositorio remoto

```{Bash}
git pull origin main
```

## Agrego los cambios y hago un commit

```{Bash}
git add .
git commit -m [nombre del commit]
```

## Pusheo el repositorio local a github

```{Bash}
git push origin main
```
