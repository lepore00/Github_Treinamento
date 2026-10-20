# Tags_Git

## O_que_e_uma_tag
Uma tag marca um commit específico do histórico, geralmente uma versão de lançamento.

## Tipos_de_tag
- Leve: apenas um nome apontando para um commit.
- Anotada: guarda autor, data e mensagem. É a mais indicada para versões.

## Comandos_principais
- `git tag -a v1.0.0 -m "Mensagem"`: cria uma tag anotada.
- `git tag`: lista as tags locais.
- `git show v1.0.0`: mostra os dados da tag e do commit marcado.
- `git push origin v1.0.0`: envia a tag ao GitHub.
- `git ls-remote --tags origin`: lista as tags do repositório remoto.

## Tags_no_Gitflow
A tag de versão é criada na `main`, depois da integração de uma `release` ou de um `hotfix`.

## Pratica_realizada
- Tag `v1.0.0` criada na `main`, no commit do merge do hotfix.
- Tag publicada no GitHub e conferida na aba Tags.