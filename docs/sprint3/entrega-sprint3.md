# Sprint 3
 
*Período:* 12/10/2026 a 27/10/2026
 
## Entregas da Sprint
 
| Trio de Desenvolvedores | Qtd. de US | US | Assunto das US |
|---|---:|---|---|
| Julio Dourado / Brenno da Silva Oliveira | - | - | - |
| André Ricardo Meyer / Giovanni Dornelas | 5 | [Issue #66](https://github.com/AppFinanceiro-GECS/koin-api/issues/66), [Issue #51](https://github.com/AppFinanceiro-GECS/koin-api/issues/51), [Issue #46](https://github.com/AppFinanceiro-GECS/koin-api/issues/46), [Issue #44](https://github.com/AppFinanceiro-GECS/koin-api/issues/44), [Issue #35](https://github.com/AppFinanceiro-GECS/koin-api/issues/35) | Cadastro aberto só na homologação, controlado por flag e sempre fechado em produção; Swagger fechado em produção e cabeçalhos HTTP reforçados; recuperação de senha pelo próprio usuário, e-mail sem diferenciar maiúsculas e uma política de senha única; atualização de dependências com vulnerabilidades conhecidas e troca de bibliotecas abandonadas; upload de HEIC, WEBP e arquivo sem extensão, validado pelo conteúdo |
| Pedro Paulo | 2 | [Issue #29](https://github.com/AppFinanceiro-GECS/koin-api/issues/29), [Issue #47](https://github.com/AppFinanceiro-GECS/koin-api/issues/47) | O trabalho focou em garantir a conformidade legal do aplicativo e a precisão temporal do sistema. Para atender à LGPD e aos requisitos da Apple e do Google, foram implementadas as rotas que dão autonomia ao usuário para exportar seu histórico completo de dados em formato JSON e para excluir sua conta de forma segura, utilizando reautenticação com senha, inativação imediata (soft delete) e registro anônimo na tabela de auditoria. Em conjunto com isso, resolvemos a falha crítica de fuso horário que registrava compras noturnas no dia seguinte, configurando o ambiente para o horário de Brasília e padronizando a geração da data local no código, o que trouxe total confiabilidade para o histórico financeiro dos usuários. |
| Rafael | 8 | [Issue #91](https://github.com/AppFinanceiro-GECS/koin-api/issues/91), [koin-api#92](https://github.com/AppFinanceiro-GECS/koin-api/pull/92), [Issue #49](https://github.com/AppFinanceiro-GECS/koin-api/issues/49), [koin-api#93](https://github.com/AppFinanceiro-GECS/koin-api/pull/93), [Issue #39](https://github.com/AppFinanceiro-GECS/koin-api/issues/39), [koin-api#94](https://github.com/AppFinanceiro-GECS/koin-api/pull/94), [Issue #33](https://github.com/AppFinanceiro-GECS/koin-api/issues/33), [koin-api#95](https://github.com/AppFinanceiro-GECS/koin-api/pull/95) | Remoção de job morto no scheduler que quebrava o boot com ImportError; bloqueio progressivo de login por e-mail, sem punir usuários atrás do mesmo IP (CGNAT de operadora móvel); validação de valor e data de transações, e correção do cálculo de fechamento/vencimento de fatura em meses de 29 a 31 dias; correção do erro 500 na listagem de transações quando o usuário tem compra no cartão de crédito |
| Ana Luiza Pfeilsticker, Gabriel Souza / João V. Farias | 2 | [koin-app#27](https://github.com/AppFinanceiro-GECS/koin-app/issues/27), [koin-app#28](https://github.com/AppFinanceiro-GECS/koin-app/issues/28) | Fluxo de pagamento de faturas e avisos de duplicação em faturas |
 
---
 
## Resumo
 
- *Líder da Apresentação*: Rafael Ferreira Leandro
- *Link Slides*: https://canva.link/5djqp29jn047hu7
- *Total de US concluídas:* 15
- *Início da Sprint:* 12/10/2026
- *Fim da Sprint:* 27/10/2026
