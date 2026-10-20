# Aula_09_Revisao_de_codigo

## Objetivo
Aprender a revisar uma alteração antes de integrá-la à `main`, verificando clareza, erros e aderência ao objetivo do Pull Request.

## Pre_requisitos
- Saber criar branches e fazer commits.
- Saber publicar uma branch no GitHub.
- Saber abrir e integrar um Pull Request (Aula_08).

## O_que_e_revisao_de_codigo
É a etapa em que outra pessoa (ou você mesmo, com um olhar crítico) lê as alterações de um Pull Request antes do merge. O objetivo é melhorar a qualidade e evitar erros, não criticar quem escreveu.

## Pontos_a_verificar
- **Objetivo:** a alteração resolve o que o Pull Request propõe?
- **Clareza:** nomes, textos e instruções são fáceis de entender?
- **Consistencia:** a estrutura segue o padrão dos outros materiais?
- **Riscos:** há algo que possa apagar, expor ou quebrar informações?

## Como_escrever_um_comentario_construtivo
Um bom comentário é respeitoso, específico e explica o motivo.

| Comentário fraco | Comentário construtivo |
|---|---|
| Está confuso. | No trecho "Etapas do fluxo", a etapa 3 não explica qual comando publica a branch. Poderia incluir o comando? |
| Nome ruim. | O arquivo `Teste` não indica o assunto. Sugiro `Git_teste_de_isolamento` para seguir o padrão do portfólio. |

## Tipos_de_resultado_de_uma_revisao
- **Comment:** apenas comentários, sem aprovar nem bloquear.
- **Approve:** aprova a alteração.
- **Request changes:** pede ajustes antes do merge.

## Exemplo_cotidiano
Revisar um Pull Request é como pedir a um colega para ler um e-mail importante antes de você enviá-lo: ele pode apontar erros de digitação, trechos confusos ou informações faltando.

## Comentario_para_melhorar
O nome do arquivo Teste poderia ser mais descritivo. Sugiro Git_teste_de_isolamento, pois indica o assunto do material.

Este comentário está incompleto de propósito: não diz qual nome, nem por que deveria mudar. Será usado na simulação de revisão desta aula.

## Nesta_aula
Criei a branch `09_Revisao_de_codigo`, documentei os critérios de revisão e vou abrir um Pull Request para praticar comentários e ajustes.