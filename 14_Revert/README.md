# Git revert

## O que é

O `git revert` desfaz as alterações de um commit criando um **novo commit** com o efeito contrário. O commit original continua no histórico.

## Quando usar

- Quando o commit já foi enviado ao GitHub ou compartilhado com outras pessoas.
- Quando você quer manter o histórico completo e transparente.

## Comando principal

git revert HEAD

- `HEAD` indica o commit mais recente da branch.
- Também é possível informar o código de outro commit: `git revert <codigo_do_commit>`.

## O que foi praticado

1. Criei a branch `14_Revert` a partir da `develop`.
2. Criei o arquivo `Pratica_revert.md` e fiz o commit `Git_preparar_pratica_revert`.
3. Adicionei uma linha ao arquivo e fiz o commit `Git_adicionar_linha_para_revert`.
4. Executei `git revert HEAD` para desfazer o segundo commit.
5. Conferi que a linha foi removida e que o histórico foi preservado.

## Resultado

O Git criou um novo commit de reversão. O arquivo voltou ao estado anterior, e os dois commits originais continuam no histórico.

## Diferença para outros comandos

- `git revert`: cria um novo commit que desfaz outro e preserva o histórico.
- `git reset`: move a branch para um commit anterior e pode reescrever o histórico.