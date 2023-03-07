# Resumo Comandos Git Úteis (Bash)
## Introdução
Este documento serve como guia resumindo para usar o git nativamente através de sua interface (bash). Os comandos listados e suas descrições são de acordo com  minha necessidade pessoal.
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
git branch
```
- Alterar para outra branch:
```
git checkout NOME_DA_BRANCH
```
- Apagar uma branch (localmente):
```
git branch -D NOME_DA_BRANCH
```

- Renomear a branch local atual:
```
git branch -m novo-nome-da-branch
```
- Renomear uma branch local a partir de outra:
```
git branch -m nome-atual novo-nome
```

- Tornar sua branch local igual ao master remoto:
```
git fetch origin && git reset --hard origin/master && git clean -f
```

-Exibir os conflitos com a branch remota:
```
git diff
```



<!-- ### REFERÊNCIAS:
- https://www.atlassian.com/br/git/tutorials/what-is-version-control 
- https://opensource.com/article/20/4/git-merge-conflict
- https://www.treinaweb.com.br/blog/comandos-do-git-que-voce-precisa-conhecer-parte-1#:~:text=Para%20renomear%20a%20sua%20atual,m%20%2C%20passando%20o%20novo%20nome.

-->
