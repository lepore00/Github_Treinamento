# Git stash

O `git stash` guarda temporariamente alterações ainda não commitadas para deixar a árvore de trabalho limpa. As alterações podem ser recuperadas depois.

## Comandos praticados

- `git stash push -u -m "Pratica_git_stash"`: guarda as alterações, incluindo arquivos não rastreados (`-u`), e adiciona uma mensagem.
- `git stash list`: lista os stashes guardados.
- `git stash pop`: recupera o stash mais recente e o remove da lista.
- `git status`: verifica o estado da árvore de trabalho.

## Prática

Criamos o arquivo `Pratica_stash.md`, guardamos a alteração com `git stash`, conferimos a lista e recuperamos o arquivo com `git stash pop`. Depois, adicionamos o arquivo ao Git e fizemos o commit.