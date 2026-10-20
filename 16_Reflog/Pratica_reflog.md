# Aula 16 — git reflog

## Objetivo
Consultar o histórico local de movimentações do HEAD e entender como o reflog pode ajudar a localizar commits.

## Comando praticado
```bash
git reflog
```
## Inspeção de uma entrada do reflog
Usei `git reflog -5` para consultar as cinco movimentações mais recentes do HEAD e `git show "HEAD@{3}"` para inspecionar a entrada correspondente.
O comando `git show` exibiu os detalhes do commit `Git_documentar_reset`, incluindo o arquivo alterado. Ele apenas consultou o commit, sem modificar a branch ou os arquivos.

## Observação
O reflog registra movimentações recentes do HEAD no repositório local. As entradas são identificadas como `HEAD@{0}`, `HEAD@{1}` e assim por diante, da mais recente para a mais antiga.