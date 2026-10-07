# Infraestrutura do backend e homologação

**Sprint:** Sprint 2 (15/09 a 28/09)
**Grupo:** Grupo 1 — Infraestrutura, hospedagem e DevOps (Julio Dourado e Brenno da Silva Oliveira)
**Issues:** [#15](https://github.com/AppFinanceiro-GECS/koin-docs/issues/15), [#16](https://github.com/AppFinanceiro-GECS/koin-docs/issues/16), [#17](https://github.com/AppFinanceiro-GECS/koin-docs/issues/17)

## Estado atual

O Grupo 1 dividiu os repositórios e configurou o CI/CD do backend. A API está hospedada na Oracle Cloud Free Tier.

| Repositório | Conteúdo |
| --- | --- |
| [koin-api](https://github.com/AppFinanceiro-GECS/koin-api) | Backend (FastAPI) e infraestrutura (Docker, deploy) |
| [koin-app](https://github.com/AppFinanceiro-GECS/koin-app) | App mobile Android/iOS (React Native + Expo) |
| [koin-docs](https://github.com/AppFinanceiro-GECS/koin-docs) | Documentação do projeto |

## Importante: a `main` do backend é a homologação

A branch `main` do `koin-api` está vinculada ao deploy de homologação. Podem mexer sem medo: basta abrir PR para a `main`, e os testes rodam automaticamente (gitleaks, lint, testes e build da imagem). Depois do merge, a homologação é atualizada sozinha em alguns minutos. Se a versão nova não subir, o deploy volta para a anterior.

A branch `prod` é a produção e só recebe PRs de promoção `main` → `prod`.

## Links

| Ambiente | Branch | Swagger |
| --- | --- | --- |
| Homologação | `main` | https://hml.144-22-232-63.sslip.io/docs |
| Produção | `prod` | https://api.144-22-232-63.sslip.io/docs (sobe na primeira promoção) |

## Usuário admin da homologação

Existe um usuário admin para testes, com login na rota `POST /api/v1/auth/login`. As credenciais **não** ficam neste repositório, porque ele é público: peça ao Grupo 1 no grupo do time.

Para usar no Swagger: faça o login em `/api/v1/auth/login`, copie o `access_token` e cole em **Authorize** (cadeado no topo da página).

## Mais detalhes

- Fluxo de branches e o que o CI cobra: [CONTRIBUTING do koin-api](https://github.com/AppFinanceiro-GECS/koin-api/blob/main/CONTRIBUTING.md)
- Como o deploy funciona, operação e rollback: [DEPLOY.md](https://github.com/AppFinanceiro-GECS/koin-api/blob/main/docs/infra/DEPLOY.md)
