# Comandos para ver los logs

Para ver los comandos en una sola linea:

```bash
git log --oneline
```

```bash
git log --decorate --all --graph
```

Un log potente

```bash
git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"
```
