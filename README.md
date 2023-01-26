# Resumo Comandos Git Úteis (Bash)
## Introdução
Este documento serve como guia resumindo para usar o git nativamente através de sua interface nativa (bash). Os comandos listadpos e suas descrições são de acordo com  minha necessidade pessoal.
## Comandos de Download e Upload
- Clonar um repositório:

```
git clone LINK_DO_REPOSITÓRIO.git
```

- Subir suas alterações para este repositório (para a ramificação principal):
```
git status
```
```
git add .
```
```
git commit -m"SUA_MENSAGEM"
```
```
git push
```

Esses comandos podem ser combinados da seguinte forma:

```
$ git status && git add . && git commit -m"SUA_MENSAGEM" && git push

```
- Baixar as alterções remotas:
```
git add .
```
```
git commit -m"SUA_MENSAGEM"
```
```
git pull
```
Esses comandos podem ser combinados da seguinte forma:

```
$ git add . && git commit -m"SUA_MENSAGEM" && git pull

```
- Reverter as alterações para um estado de commit anterior (localmente)
```
git log
```
> :bulb: **Dica:** Pra sair do log digite `:q`

```
git commit -m"SUA_MENSAGEM"
```
```
git reset HASH_DO_SEU_COMMIT        
```
```
git clean -n
```

```
git clean -f
```

- Criar uma nova branch e alterar para ela:
```
git checkout -b SUA_NOVA_BRANCH
```
- Listar as branchs disponíveis:
```
git clean -n
```
- Alterar para outra branch:
```
git checkout NOME_DA_BRANCH
```
Desfazer as alterções da branch anterior:

```
$ git add . && git commit -m"SUA_MENSAGEM" git reset
```
- Apagar uma branch (localmente):
```
git branch -D NOME_DA_BRANCH
```
