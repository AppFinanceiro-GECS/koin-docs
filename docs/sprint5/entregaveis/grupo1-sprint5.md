# Grupo 1 na Sprint 5: fluxos principais e entrega

**Sprint:** Sprint 5 (12/11 a 28/11/2026)
**Grupo:** Grupo 1 — Infraestrutura, hospedagem e DevOps (Julio Dourado e Brenno da Silva Oliveira)

Com a API pronta na Sprint 4, o Grupo 1 levou ao app os fluxos que mais geram valor para o público do Koin (casais e famílias que gastam no cartão) e fechou a entrega ao cliente. Todos os fluxos foram validados no emulador Android contra a homologação, com usuários de teste.

## O cartão nasce da fatura

| PR | O que mudou |
|---|---|
| [koin-app#31](https://github.com/AppFinanceiro-GECS/koin-app/pull/31), [koin-api#130](https://github.com/AppFinanceiro-GECS/koin-api/pull/130) | Escanear a fatura com a câmera; leitura completa de PDFs com lixo antes do cabeçalho; recusa de documento que não é financeiro, com mensagem clara |
| [koin-app#32](https://github.com/AppFinanceiro-GECS/koin-app/pull/32), [koin-api#131](https://github.com/AppFinanceiro-GECS/koin-api/pull/131) | Excluir e editar cartão com segurança e permissões da família |
| [koin-app#33](https://github.com/AppFinanceiro-GECS/koin-app/pull/33), [koin-api#132](https://github.com/AppFinanceiro-GECS/koin-api/pull/132) | Cartão reconhecido pela fatura (final e banco) ou cadastrado em um toque; projeção das parcelas; novo Início e tutorial de boas-vindas |
| [koin-app#36](https://github.com/AppFinanceiro-GECS/koin-app/pull/36), [koin-api#135](https://github.com/AppFinanceiro-GECS/koin-api/pull/135) | Cartões com a cor e o logo do banco; quanto está comprometido em cada cartão |

Documento: [O cartão nasce da fatura](../../produto/fluxo-cartao-pela-fatura.md).

## Comprovantes

| PR | O que mudou |
|---|---|
| [koin-api#133](https://github.com/AppFinanceiro-GECS/koin-api/pull/133), [koin-app#34](https://github.com/AppFinanceiro-GECS/koin-app/pull/34) | Comprovante de pagamento acha a fatura aberta e oferece marcá-la como paga; compra com o final do cartão vai para a fatura certa, e final desconhecido oferece cadastrar o cartão |

## Família

| PR | O que mudou |
|---|---|
| [koin-api#134](https://github.com/AppFinanceiro-GECS/koin-api/pull/134), [koin-app#35](https://github.com/AppFinanceiro-GECS/koin-app/pull/35) | Divisão do mês: quem pagou o quê, a parte de cada um, quem deve a quem e o acerto; divisão igual ou proporcional à renda; entrar na família com o código, já tendo conta |
| [koin-api#136](https://github.com/AppFinanceiro-GECS/koin-api/pull/136), [koin-app#37](https://github.com/AppFinanceiro-GECS/koin-app/pull/37) | Cartão da casa: todas as compras do cartão entram na divisão, sem marcar uma a uma |

Documento: [Família, quem pagou o quê e o acerto](../../produto/familia-divisao.md).

## Qualidade e segurança

| PR | O que mudou |
|---|---|
| [koin-api#137](https://github.com/AppFinanceiro-GECS/koin-api/pull/137) | Swagger fechado em produção; respostas sem cabeçalhos que expõem o servidor |
| [koin-app#38](https://github.com/AppFinanceiro-GECS/koin-app/pull/38) | Tipos do app gerados do OpenAPI da API, com aviso no CI quando ficam desatualizados |
| [koin-app#39](https://github.com/AppFinanceiro-GECS/koin-app/pull/39) | Cores com contraste AA e checklist de acessibilidade no template de PR |
| [koin-app#40](https://github.com/AppFinanceiro-GECS/koin-app/pull/40) | Expo 58.0.25, que destravou o CI de todos os PRs do app |

## Entrega ao cliente

| PR | O que mudou |
|---|---|
| [koin-docs#31](https://github.com/AppFinanceiro-GECS/koin-docs/pull/31) | [Entrega do projeto](../../entrega/README.md) e [custos operacionais](../../entrega/custos.md) |
| [koin-docs#27](https://github.com/AppFinanceiro-GECS/koin-docs/pull/27) a [#30](https://github.com/AppFinanceiro-GECS/koin-docs/pull/30) | Documentos de produto de cada fluxo |
| — | Issues de hospedagem e infra encerradas (koin-api#17, #21–#27, #30, #31, #52; koin-app#11; koin-docs#20), cada uma apontando para o documento de entrega |
| — | [Documento da reunião com o cliente](../../entrega/reuniao-cliente.md) |
