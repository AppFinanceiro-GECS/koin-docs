# Grupo 1 nas cinco sprints

**Grupo:** Grupo 1 — Infraestrutura, hospedagem e DevOps
**Integrantes:** Julio Dourado e Brenno da Silva Oliveira
**Período:** 01/09 a 28/11/2026 (5 sprints de cerca de 15 dias)

Os commits do grupo são do Julio, com o Brenno como coautor em todos.

| Sprint | Período | Foco | Principais entregas |
|---|---|---|---|
| 1 | 01/09 a 08/09 | Viabilidade | Viabilidade técnica do iOS ([koin-docs#7](https://github.com/AppFinanceiro-GECS/koin-docs/pull/7)) e do Android ([koin-docs#9](https://github.com/AppFinanceiro-GECS/koin-docs/pull/9)); ata da reunião de alinhamento ([koin-docs#8](https://github.com/AppFinanceiro-GECS/koin-docs/pull/8)) |
| 2 | 21/09 a 07/10 | Infraestrutura | Divisão do monorepo em `koin-api`, `koin-app` e `koin-docs`; VM na Oracle Cloud; CI/CD com deploy automático e volta para a versão anterior se falhar; homologação contínua do app pelo EAS Update; SDK 58; correções da leitura de faturas; auditoria do projeto em 30/09, transformada em 6 épicos e 45 issues priorizadas ([detalhes](../../sprint2/entregaveis/infra-backend-homologacao.md)) |
| 3 | 12/10 a 27/10 | Arquitetura e processo | Diagramas de arquitetura, decisões técnicas, fluxo do aplicativo, guia de contribuição com padrões de branch, commit e PR ([Sprint 3](../../sprint3/entrega-sprint3.md)) |
| 4 | 28/10 a 11/11 | API pronta para produção | 18 PRs: sessões revogáveis, contrato de erro, IA resiliente, etapas da leitura, retenção (LGPD), push, observabilidade, CI com Postgres, Trivy e smoke E2E ([detalhes](../../sprint4/entregaveis/grupo1-sprint4.md)) |
| 5 | 12/11 a 28/11 | Fluxos de valor e entrega | 23 PRs: cartão pela fatura, comprovantes, família com divisão e cartão da casa, segurança e acessibilidade, documentação de produto, entrega do projeto e custos ([detalhes](grupo1-sprint5.md)) |

## Números no fim do projeto

| | |
|---|---|
| Testes da API | 582, com cobertura de 59% (mínimo de 55% no CI) |
| Ambientes | Homologação no ar desde a Sprint 2, com deploy a cada merge |
| Custo de IA medido | US$ 0,00427 por documento lido |
| Custo estimado | R$ 248,63 por mês para 1.000 usuários ([custos](../../entrega/custos.md)) |

## O que fica para o cliente

Tudo o que é preciso para continuar está no [documento de entrega](../../entrega/README.md): contas a transferir, servidor (no ar até 31/12/2026), chaves e o que falta para publicar nas lojas.
