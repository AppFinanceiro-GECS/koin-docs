# Custos operacionais do Koin

*Referência:* novembro de 2026 · câmbio de R$ 5,50 por US$ 1
*Planilha editável:* [custos-operacionais.xlsx](custos-operacionais.xlsx) (as células amarelas são os parâmetros; o resto recalcula) · [versão em PDF](custos-operacionais.pdf)
*Issue:* [koin-docs#21](https://github.com/AppFinanceiro-GECS/koin-docs/issues/21)

## Resumo

Cenário de exemplo: **1.000 usuários ativos**, cada um enviando **5 documentos por mês** (2 faturas + 3 cupons ou comprovantes).

| | Valor |
|---|---:|
| Custo fixo por mês | R$ 131,21 |
| Custo variável por mês | R$ 117,43 |
| **Custo total por mês** | **R$ 248,63** |
| Custo por usuário ativo por mês | R$ 0,25 |
| Custo que cada usuário a mais acrescenta | R$ 0,12 |
| Fixo do 1º ano (com taxas únicas) | R$ 1.712,00 |
| **Total do 1º ano** (fixo + 12 meses de variável) | **R$ 3.121,10** |

O principal custo variável é a **leitura de documentos por IA**. Ela foi medida na homologação: média de 25 leituras reais com o Gemini 3.5 Flash-Lite, com cerca de 6,8 mil tokens de entrada e 1,1 mil de saída por documento, ou seja, **US$ 0,00427 por documento**.

## Custos fixos

Não dependem de quantas pessoas usam o app.

| Item | Para que serve | Cobrança | Valor | Por mês | Observação |
|---|---|---|---:|---:|---|
| Apple Developer Program | Publicar e manter o app na App Store | Anual | US$ 99 (R$ 544,50) | R$ 45,38 | Obrigatório para iOS; sem renovar, o app sai da loja |
| Google Play Console | Publicar na Play Store | Única vez | US$ 25 (R$ 137,50) | – | Entra só no 1º ano |
| Domínio .com.br | Endereço do app e da API | Anual | R$ 40,00 | R$ 3,33 | Registro.br |
| Servidor (API + banco) | Onde o sistema roda | Mensal | US$ 15 | R$ 82,50 | Hoje roda no Oracle Cloud Always Free (veja abaixo). O valor fica como reserva para uma VPS de US$ 8 a 25 por mês |
| Publicação do app | Gerar o app e enviar atualizações | Mensal | US$ 0 | – | Expo EAS gratuito (15 builds Android + 15 iOS por mês) |
| E-mail automático | Confirmação de conta, senha | Mensal | US$ 0 | – | Resend gratuito: até 3 mil por mês (100 por dia) |
| Armazenamento | Faturas enviadas e backups | Mensal | US$ 0 | – | 10 a 20 GB grátis (Oracle ou Cloudflare R2) |
| DNS, segurança e monitoramento | Proteção e aviso de falhas | Mensal | US$ 0 | – | Cloudflare, Sentry e uptime gratuitos |
| **Total fixo por mês** | | | | **R$ 131,21** | Anuais divididos por 12 |

> **Sobre o servidor:** a VM de homologação está na conta Oracle pessoal do Julio, no Always Free, e fica no ar até **31/12/2026**. A partir de 2027, o servidor passa a ser um custo real: uma conta Oracle própria (que pode continuar no gratuito) ou uma VPS. Por isso os R$ 82,50 já entram no total.

## Custos variáveis

Crescem com o uso. Valores do cenário de 1.000 usuários.

| Item | Unidade | Preço | Quantidade por mês | Grátis por mês | Por mês | Observação |
|---|---|---:|---:|---:|---:|---|
| Leitura de faturas e cupons por IA | documento | US$ 0,00427 | 5.000 | 0 | R$ 117,43 | Gemini no plano pago, obrigatório em produção: no gratuito, o Google pode usar os dados enviados |
| Armazenamento acima do grátis | GB guardado | US$ 0,02 | 4,9 | 10 | – | Cloudflare R2; arquivos guardados por 30 dias |
| E-mails automáticos | e-mail | US$ 0 | 2.000 | 3.000 | – | Acima de 100 por dia: Resend Pro |
| Notificações no celular | envio | US$ 0 | 10.000 | ilimitado | – | Expo Push é gratuito |
| **Total variável por mês** | | | | | **R$ 117,43** | |

## Como o custo escala

O custo por usuário cai à medida que a base cresce, porque o fixo é diluído. O custo da IA cresce em linha reta.

| Usuários ativos | Fixo por mês | IA por mês | Total por mês | Por usuário |
|---:|---:|---:|---:|---:|
| 100 | R$ 131,21 | R$ 11,74 | R$ 142,95 | R$ 1,43 |
| 1.000 | R$ 131,21 | R$ 117,43 | R$ 248,63 | R$ 0,25 |
| 10.000 | R$ 131,21 | R$ 1.174,25 | R$ 1.305,46 | R$ 0,13 |

Com 10 mil usuários, somam-se cerca de R$ 4,40 de armazenamento (40 GB acima do grátis). Também passa a valer o Resend Pro, porque serão uns 20 mil e-mails por mês, acima de 100 por dia. Os upgrades abaixo não estão na tabela.

## Upgrades opcionais

Não estão no total. Contratar quando o uso pedir.

| Item | Quando contratar | Por mês |
|---|---|---:|
| Resend Pro (e-mail) | Mais de 100 e-mails por dia | US$ 20 (R$ 110,00) |
| Expo EAS Starter | Fila prioritária para gerar o app | US$ 19 (R$ 104,50) |
| Sentry Team | Muitos usuários e alertas detalhados | US$ 26 (R$ 143,00) |

## Fontes

Preços públicos de Apple, Google Play, Registro.br, Oracle Cloud, Expo, Resend, Cloudflare e Google Gemini, levantados em 30/09/2026 e revisados em 04/11/2026. O custo de IA foi medido na homologação em novembro de 2026. Confirme o câmbio e os preços na data da contratação.
