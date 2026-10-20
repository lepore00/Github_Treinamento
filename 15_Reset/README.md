
## O que é o git reset
O `git reset` move a ponta da branch (o `HEAD`) para outro commit. Dependendo do modo, ele também altera o stage e os arquivos da pasta de trabalho.

## Os três modos

| Modo | Commit | Stage | Arquivos na pasta |
|------|--------|-------|-------------------|
| `--soft` | Desfeito | Mantém as alterações | Mantidos |
| `--mixed` (padrão) | Desfeito | Alterações saem do stage | Mantidos |
| `--hard` | Desfeito | Limpo | Alterações descartadas |

## Comandos praticados

git reset --soft HEAD~1
git reset --mixed HEAD~1
git reset --hard HEAD

- `HEAD~1`: o commit anterior ao atual.
- `HEAD`: o commit atual.

## Prática realizada
- Arquivo de teste: `15_Reset/Pratica_reset.md`.
- Commits de teste: `Git_preparar_pratica_reset` e `Git_adicionar_alteracao_para_reset`.
- Com `--soft`, o commit foi desfeito e a alteração continuou no stage.
- Com `--mixed`, o commit foi desfeito e a alteração ficou fora do stage.
- Com `git diff`, confirmei que a alteração continuava no arquivo.
- Com `--hard HEAD`, a alteração não commitada foi descartada e a árvore ficou limpa.

## Aprendizados
- Cada execução de `git reset --soft HEAD~1` desfaz mais um commit. Executar duas vezes remove dois commits.
- `git status` mostra o resultado de cada modo: "Changes to be committed" (stage) ou "Changes not staged for commit" (fora do stage).
- `git diff` mostra o que está modificado fora do stage.
- `--hard` é o modo mais arriscado, pois descarta alterações locais não commitadas.
- Antes de usar `--hard`, salve o que for importante em um commit ou use `git stash`.
- Para commits já publicados no GitHub, o `git revert` é mais seguro, pois não reescreve o histórico.

## Cuidados
- Use `git status` antes de qualquer `git reset`.
- Evite `git reset --hard` em alterações importantes.
- Evite reescrever o histórico de commits já enviados ao GitHub.