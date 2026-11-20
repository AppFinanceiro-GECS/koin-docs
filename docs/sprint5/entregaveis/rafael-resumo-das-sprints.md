# Rafael nas cinco sprints

**Integrante:** Rafael Ferreira Leandro
**Frente:** Backend (manutenção corretiva e evolutiva do `koin-api`)
**Período:** 01/09 a 28/11/2026 (5 sprints de cerca de 15 dias)

| Sprint | Período | Foco | Principais entregas |
|---|---|---|---|
| 1 | 01/09 a 08/09 | Proposta de MVP | Consolidação da proposta de MVP e registro das entregas do grupo ([koin-docs#12](https://github.com/AppFinanceiro-GECS/koin-docs/pull/12)) |
| 2 | 21/09 a 07/10 | Notificações e correções de e-mail | Entrega de notificações pendentes por e-mail via job agendado no backend, com retentativa automática em caso de falha de envio ([Issue #69](https://github.com/AppFinanceiro-GECS/koin-api/issues/69), [koin-api#70](https://github.com/AppFinanceiro-GECS/koin-api/pull/70)); correção da logo quebrada e do domínio desatualizado (biveto.com) nos templates de e-mail ([Issue #76](https://github.com/AppFinanceiro-GECS/koin-api/issues/76), [koin-api#78](https://github.com/AppFinanceiro-GECS/koin-api/pull/78)) |
| 3 | 12/10 a 27/10 | Correção de bugs do backlog de manutenção | Remoção de job morto no scheduler que quebrava o boot da API com `ImportError` ([Issue #91](https://github.com/AppFinanceiro-GECS/koin-api/issues/91), [koin-api#92](https://github.com/AppFinanceiro-GECS/koin-api/pull/92)); bloqueio progressivo de login por e-mail, sem punir usuários atrás do mesmo IP — CGNAT de operadora móvel ([Issue #49](https://github.com/AppFinanceiro-GECS/koin-api/issues/49), [koin-api#93](https://github.com/AppFinanceiro-GECS/koin-api/pull/93)); validação de valor e data de transações, e correção do cálculo de fechamento/vencimento de fatura em meses de 29 a 31 dias ([Issue #39](https://github.com/AppFinanceiro-GECS/koin-api/issues/39), [koin-api#94](https://github.com/AppFinanceiro-GECS/koin-api/pull/94)); correção do erro 500 na listagem de transações quando o usuário tem compra no cartão de crédito ([Issue #33](https://github.com/AppFinanceiro-GECS/koin-api/issues/33), [koin-api#95](https://github.com/AppFinanceiro-GECS/koin-api/pull/95)) |
| 4 | 28/10 a 11/11 | Testes e validação com o cliente | Testes manuais dos fluxos do app e participação na [reunião de validação com o cliente](https://youtu.be/m4sojK-9o1E) ([detalhes](../../sprint4/entrega-sprint4.md)) |
| 5 | 12/11 a 28/11 | Documentação de entrega e apresentação final | Resumo do projeto para apresentação ao cliente final (como o produto funciona, onde está hospedado e como testar) e roteiro de demonstração das funcionalidades do app |

## Números (Sprints 2 e 3, trabalho com issue e PR vinculados)

| | |
|---|---|
| Issues abertas e resolvidas | 6 ([#69](https://github.com/AppFinanceiro-GECS/koin-api/issues/69), [#76](https://github.com/AppFinanceiro-GECS/koin-api/issues/76), [#91](https://github.com/AppFinanceiro-GECS/koin-api/issues/91), [#49](https://github.com/AppFinanceiro-GECS/koin-api/issues/49), [#39](https://github.com/AppFinanceiro-GECS/koin-api/issues/39), [#33](https://github.com/AppFinanceiro-GECS/koin-api/issues/33)) |
| Pull Requests mergeados | 6 ([#70](https://github.com/AppFinanceiro-GECS/koin-api/pull/70), [#78](https://github.com/AppFinanceiro-GECS/koin-api/pull/78), [#92](https://github.com/AppFinanceiro-GECS/koin-api/pull/92), [#93](https://github.com/AppFinanceiro-GECS/koin-api/pull/93), [#94](https://github.com/AppFinanceiro-GECS/koin-api/pull/94), [#95](https://github.com/AppFinanceiro-GECS/koin-api/pull/95)) |
| Testes automatizados adicionados | Cobrindo notificação por e-mail, bloqueio progressivo de login, validação de valor/data de transação, cálculo de fatura e listagem de transações com cartão |

## O que ficou pronto

Todo o trabalho seguiu o fluxo completo de manutenção corretiva: issue documentada (causa, evidência e critério de aceite) → branch própria → implementação com teste automatizado → validação manual contra o ambiente real → Pull Request revisado via CI/CD. Detalhes de cada entrega em [Sprint 2](../../sprint2/entrega-sprint2.md) e [Sprint 3](../../sprint3/entrega-sprint3.md).
