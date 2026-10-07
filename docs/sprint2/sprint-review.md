# Ata de Reunião — Alinhamento Sprint 2

**Data:** [completar]
**Horário:** [completar]
**Plataforma:** Google Meet

## Pauta

Alinhamento do andamento das tarefas de cada área/grupo na Sprint 2
(15/09 a 28/09), conforme os itens já em acompanhamento nas issues do
GitHub de cada grupo.

## Evidência da reunião

> Adicionar o print da reunião em `docs/assets/reuniao-alinhamento-sprint2.png`
> e trocar esta nota pela imagem.

## Entregas da Sprint

Atividades já concluídas por trio/dupla até o momento da reunião, uma por
linha, com a evidência correspondente. Cada grupo deve preencher sua própria
seção seguindo o padrão da tabela abaixo.

### Grupo 1 — Infraestrutura, hospedagem e DevOps

Detalhamento completo nas issues [#15](https://github.com/AppFinanceiro-GECS/koin-docs/issues/15), [#16](https://github.com/AppFinanceiro-GECS/koin-docs/issues/16) e [#17](https://github.com/AppFinanceiro-GECS/koin-docs/issues/17). Estado atual e como usar a homologação em [infra-backend-homologacao.md](entregaveis/infra-backend-homologacao.md).

| Nome do Trio/Dupla | Atividade | Evidência |
| --- | --- | --- |
| Julio Dourado e Brenno da Silva Oliveira | Dividiu o monorepo em `koin-api` (backend + infra) e `koin-app` (mobile), com branches `main` (homologação) e `prod` (produção), e renomeou os repositórios para Koin | [#15](https://github.com/AppFinanceiro-GECS/koin-docs/issues/15) |
| Julio Dourado e Brenno da Silva Oliveira | Hospedou o backend na Oracle Cloud Free Tier (VM ARM em São Paulo, HTTPS automático) | [#16](https://github.com/AppFinanceiro-GECS/koin-docs/issues/16), [Swagger da homologação](https://hml.144-22-232-63.sslip.io/docs) |
| Julio Dourado e Brenno da Silva Oliveira | Configurou o CI/CD do backend: testes em todo PR e deploy automático da `main` na homologação e da `prod` na produção | [#17](https://github.com/AppFinanceiro-GECS/koin-docs/issues/17), [ci.yml](https://github.com/AppFinanceiro-GECS/koin-api/blob/main/.github/workflows/ci.yml) |
| Julio Dourado e Brenno da Silva Oliveira | Extraiu o backend e a infra do monorepo `biveto-fin` para o `koin-api` e publicou o app mobile (React Native + Expo) no `koin-app` | [koin-api f6a87e2](https://github.com/AppFinanceiro-GECS/koin-api/commit/f6a87e2), [koin-app 1af3a78](https://github.com/AppFinanceiro-GECS/koin-app/commit/1af3a78) |
| Julio Dourado e Brenno da Silva Oliveira | Adicionou varredura de segredos (gitleaks via CLI em container) ao CI do backend e do app, com schemas zod compatíveis com v3 e v4 no app | [koin-api fa4c08a](https://github.com/AppFinanceiro-GECS/koin-api/commit/fa4c08a), [koin-app 659674e](https://github.com/AppFinanceiro-GECS/koin-app/commit/659674e) |
| Julio Dourado e Brenno da Silva Oliveira | Criou a branch `prod` no fluxo do CI (`main` → `prod`) nos dois repositórios | [koin-api e36d609](https://github.com/AppFinanceiro-GECS/koin-api/commit/e36d609), [koin-app 7564903](https://github.com/AppFinanceiro-GECS/koin-app/commit/7564903) |
| Julio Dourado e Brenno da Silva Oliveira | Implementou o deploy automático na VM da Oracle (`main` → homologação, `prod` → produção) | [koin-api dd159ec](https://github.com/AppFinanceiro-GECS/koin-api/commit/dd159ec) |
| Julio Dourado e Brenno da Silva Oliveira | Renomeou Biveto para Koin no código e nas configs e apontou os perfis `preview` e `production` do app (EAS) para a API na Oracle | [koin-api 8ea4e8a](https://github.com/AppFinanceiro-GECS/koin-api/commit/8ea4e8a), [koin-app 1667cd6](https://github.com/AppFinanceiro-GECS/koin-app/commit/1667cd6) |
| Julio Dourado e Brenno da Silva Oliveira | Alinhou as dependências do app aos patches do Expo SDK 57 exigidos pelo `expo-doctor` | [koin-app fb52ff9](https://github.com/AppFinanceiro-GECS/koin-app/commit/fb52ff9) |

### Grupo 2 — Backend, dados e IA

Detalhamento completo na [issue #X](https://github.com/AppFinanceiro-GECS/koin-docs/issues).

| Nome do Trio/Dupla | Atividade | Evidência |
| --- | --- | --- |
| [nome do integrante ou da dupla] | [atividade concluída] | [link para o documento, PR, print ou comentário que comprova a entrega] |

### Grupo 3 — Regras de negócio e fluxos financeiros

Detalhamento completo na [issue #X](https://github.com/AppFinanceiro-GECS/koin-docs/issues).

| Nome do Trio/Dupla | Atividade | Evidência |
| --- | --- | --- |
| [nome do integrante ou da dupla] | [atividade concluída] | [link para o documento, PR, print ou comentário que comprova a entrega] |

### Grupo 4 — Produto, requisitos e frontend

Detalhamento completo na [issue #X](https://github.com/AppFinanceiro-GECS/koin-docs/issues).

| Nome do Trio/Dupla | Atividade | Evidência |
| --- | --- | --- |
| [nome do integrante ou da dupla] | [atividade concluída] | [link para o documento, PR, print ou comentário que comprova a entrega] |

### Grupo 5 — FrontEnd UI/UX

Detalhamento completo na [issue #X](https://github.com/AppFinanceiro-GECS/koin-docs/issues).

| Nome do Trio/Dupla | Atividade | Evidência |
| --- | --- | --- |
| [nome do integrante ou da dupla] | [atividade concluída] | [link para o documento, PR, print ou comentário que comprova a entrega] |

> Grupos 2 a 5: preencher com as entregas reais e remover esta nota.

## Registro

Reunião realizada para verificação do andamento das entregas de cada
grupo na Sprint 2. O status detalhado de cada atividade está refletido na
tabela acima e permanece atualizado nas respectivas issues no GitHub.
