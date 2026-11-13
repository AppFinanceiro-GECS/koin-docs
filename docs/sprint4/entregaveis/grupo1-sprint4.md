# Grupo 1 na Sprint 4: API pronta para produção

**Sprint:** Sprint 4 (28/10 a 11/11/2026)
**Grupo:** Grupo 1 — Infraestrutura, hospedagem e DevOps (Julio Dourado e Brenno da Silva Oliveira)

Nesta sprint, o Grupo 1 fechou o backlog da auditoria de 30/09 que deixava a API pronta para produção. Cada item virou um PR com testes e CI verde, e foi para a homologação no merge.

## Segurança e sessão

| PR | O que mudou |
|---|---|
| [koin-api#109](https://github.com/AppFinanceiro-GECS/koin-api/pull/109) | Sessões revogáveis: refresh token rotativo, logout de um aparelho ou de todos |
| [koin-api#113](https://github.com/AppFinanceiro-GECS/koin-api/pull/113) | Contrato de erro único (RFC 9457) com `code` estável, `request_id` e versão da API exposta |
| [koin-api#121](https://github.com/AppFinanceiro-GECS/koin-api/pull/121) | Dependências travadas com hash e política do Dependabot |

## Leitura de faturas e IA

| PR | O que mudou |
|---|---|
| [koin-api#108](https://github.com/AppFinanceiro-GECS/koin-api/pull/108) | Modelo alternativo quando o Gemini responde 503, raciocínio mínimo (mais barato) e validação dos modelos |
| [koin-api#114](https://github.com/AppFinanceiro-GECS/koin-api/pull/114) | Regra RN016: se a IA estiver fora, o envio não se perde e é processado depois |
| [koin-api#120](https://github.com/AppFinanceiro-GECS/koin-api/pull/120) | Etapas da leitura (`received`, `extracting`, `validating`, `done`) para o app mostrar o progresso |
| [koin-api#117](https://github.com/AppFinanceiro-GECS/koin-api/pull/117) | Retenção: o arquivo original da fatura é apagado depois de 30 dias (LGPD) |

## Produto e operação

| PR | O que mudou |
|---|---|
| [koin-api#111](https://github.com/AppFinanceiro-GECS/koin-api/pull/111) | `ENABLED_MODULES`: produção sobe só com os módulos do MVP |
| [koin-api#119](https://github.com/AppFinanceiro-GECS/koin-api/pull/119) | Push pelo Expo e lembrete de vencimento da fatura |
| [koin-api#112](https://github.com/AppFinanceiro-GECS/koin-api/pull/112) | E-mail fora do event loop: falha no SMTP não derruba a requisição |
| [koin-api#110](https://github.com/AppFinanceiro-GECS/koin-api/pull/110) | Link de convite copiável e usuário demo com dados para testes |
| [koin-api#124](https://github.com/AppFinanceiro-GECS/koin-api/pull/124) | Observabilidade: logs em JSON e Sentry opcional |

## Qualidade e CI

| PR | O que mudou |
|---|---|
| [koin-api#116](https://github.com/AppFinanceiro-GECS/koin-api/pull/116) | Testes também em Postgres, cobertura mínima no CI, scan da imagem (Trivy) e smoke E2E depois de cada deploy |
| [koin-api#118](https://github.com/AppFinanceiro-GECS/koin-api/pull/118) | Testes de integração do núcleo do MVP e correção dos alertas de fatura |
| [koin-api#105](https://github.com/AppFinanceiro-GECS/koin-api/pull/105), [#106](https://github.com/AppFinanceiro-GECS/koin-api/pull/106) | `main` voltou a passar no CI; migrações funcionando também no SQLite |
| [koin-api#115](https://github.com/AppFinanceiro-GECS/koin-api/pull/115) | `operationId` legível e `openapi.json` publicado pelo CI (base dos tipos gerados no app) |
| [koin-api#127](https://github.com/AppFinanceiro-GECS/koin-api/pull/127) | Coleção Bruno e roteiro de teste da homologação para os outros grupos |

## Itens da reunião da sprint

Da [ata](ata-reuniao-sprint4.md), ficaram com o Grupo 1 e foram resolvidos: hospedagem do backend, tokens, logs e observabilidade, o bug do iOS e a planilha de custos para o cliente ([custos](../../entrega/custos.md)). A publicação nas lojas e a produção dependiam do cliente e ficaram fora, porque ele decidiu não publicar neste semestre (veja a [Sprint 5](../../sprint5/entrega-sprint5.md)).
