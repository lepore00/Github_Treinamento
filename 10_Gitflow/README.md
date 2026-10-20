# Aula_10_Gitflow

## Objetivo
Entender como o Gitflow organiza o desenvolvimento em branches com funções bem definidas.

## Pré-requisitos
- Branches
- Pull Requests
- GitHub Flow

## O que é Gitflow
Gitflow é uma estratégia de organização de branches para projetos que trabalham com versões e lançamentos planejados. Cada tipo de branch tem uma função específica.

## Branches_do_Gitflow

| Branch | Função | Sai de | Volta para |
|---|---|---|---|
| main | Versão estável e publicada | - | - |
| develop | Integração da próxima versão | main | - |
| feature_nome | Nova funcionalidade | develop | develop |
| release_versao | Preparação do lançamento | develop | main e develop |
| hotfix_nome | Correção urgente em produção | main | main e develop |

## Analogia_cotidiana
Uma editora de livros:
- main: livro publicado
- develop: rascunho da próxima edição
- feature: capítulo novo
- release: revisão final antes da impressão
- hotfix: errata urgente de um livro já publicado

## Fluxo_resumido
1. Criar `develop` a partir da `main`.
2. Criar uma `feature` a partir da `develop`.
3. Finalizar a `feature` e integrá-la à `develop`.
4. Criar uma `release` a partir da `develop` para ajustes finais.
5. Integrar a `release` na `main` e na `develop`.
6. Se surgir um erro urgente em produção, criar um `hotfix` a partir da `main` e integrá-lo na `main` e na `develop`.

## Gitflow_x_GitHub_Flow
- GitHub Flow: simples, com `main` e branches curtas; ideal para entregas contínuas.
- Gitflow: mais estruturado, com versões e lançamentos planejados.

## Observacao_sobre_nomes
O padrão tradicional usa `feature/nome`. Neste portfólio, o separador é `_` (exemplo: `feature_nome`). Em projetos reais, siga o padrão definido pela equipe.

## Nesta_aula
Branch usada para documentar: `10_Gitflow`.