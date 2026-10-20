# Conflitos de merge

Um conflito de merge acontece quando o Git não consegue combinar automaticamente alterações feitas em uma mesma parte de um arquivo. Isso costuma ocorrer quando duas branches modificam a mesma linha de formas diferentes.

## Por que os conflitos acontecem?

O Git compara as alterações entre branches. Se encontrar mudanças incompatíveis na mesma linha, ele interrompe o merge para que uma pessoa escolha como o arquivo deve ficar.

## Marcadores de conflito

Ao ocorrer um conflito, o Git insere marcadores no arquivo:

- `<<<<<<<`: início de uma das versões.
- `=======`: separa as versões em conflito.
- `>>>>>>>`: fim da outra versão.

É necessário editar o arquivo, escolher ou combinar o conteúdo desejado e remover todos os marcadores.

## Prática realizada

1. Criei o arquivo `Pratica_conflito.md` na branch `12_Conflitos` com a linha `Cor_favorita: azul`.
2. Criei duas branches a partir dessa base:
   - `conflito_cor_vermelha`, alterando a cor para `vermelho`.
   - `conflito_cor_verde`, alterando a cor para `verde`.
3. Integrei a branch com a alteração `vermelho` à `develop`.
4. Ao tentar integrar a branch com a alteração `verde`, ocorreu um conflito, pois as duas branches modificaram a mesma linha.
5. Resolvi o conflito mantendo `Cor_favorita: verde`, removi os marcadores e enviei a resolução ao GitHub.
6. Após a resolução, o PR pôde ser integrado à `develop`.

## Comandos utilizados

```bash
git switch develop
git pull origin develop
git switch conflito_cor_verde
git merge develop
```

Após editar o arquivo e resolver o conflito:

```bash
git add 12_Conflitos/Pratica_conflito.md
git status
git commit -m "Git_resolver_conflito_cor"
git push
```

## O que aprendi

- Conflitos são situações normais em projetos com alterações paralelas.
- O Git sinaliza o trecho que precisa de decisão manual.
- É importante revisar o conteúdo e remover os marcadores antes de concluir o merge.
- Depois de resolver o conflito, é necessário registrar e enviar a resolução para atualizar o Pull Request.