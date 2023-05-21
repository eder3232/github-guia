# Comandos útiles en ramas

## Cambiar el nombre de la rama por defecto al crear un proyecto de git

Para cambiar de rama permanentemente:

```{Bash}
git config --global init.defaultBranch <name>
```

Se sugiere que sea main.

## Ver el nombre de la rama actual

```{Bash}
git branch --show-current
```

## Cambiar el nombre de una rama

```{Bash}
git branch -m master main
```
