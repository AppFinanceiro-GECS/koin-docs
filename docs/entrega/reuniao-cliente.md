# Reunião de entrega com o cliente

**Projeto:** Koin, app de finanças para casais e famílias
**Apresentação final:** 28/11/2026
**Grupo responsável pela entrega:** Grupo 1 (Julio Dourado e Brenno da Silva Oliveira)

Documento curto para conduzir a reunião. Os detalhes técnicos estão na [entrega do projeto](README.md) e os números em [custos](custos.md).

## 1. Pauta

1. O que foi construído (10 min, com demonstração no celular)
2. Decisão sobre a publicação (5 min)
3. Custos para operar (5 min)
4. Entrega das contas e do código (15 min)
5. Próximos passos e prazos (5 min)

## 2. O que foi construído

O Koin lê a fatura do cartão (PDF ou foto) com IA e responde às três perguntas de quem divide as contas de casa: **quanto gastei no cartão, quem da casa gastou o quê e quem deve a quem**.

| Fluxo | O que a pessoa faz |
|---|---|
| Fatura | Fotografa ou envia o PDF; o app reconhece o cartão (ou cadastra em um toque), lista as compras e as parcelas, e a pessoa só confere |
| Comprovantes | Envia o comprovante de pagamento e a fatura é marcada como paga; uma compra com o final do cartão cai na fatura certa |
| Família | Convida quem divide as contas; o app mostra quem pagou o quê, a parte de cada um (igual ou pela renda) e "Você paga R$ 120 para Paula"; o acerto é registrado depois do Pix |
| Cartão da casa | Marca um cartão como da casa e todas as compras dele entram na divisão |
| Básico | Contas, transações, parcelamentos, resumo do mês, notificações, exclusão e exportação de dados (LGPD) |

**Demonstração:** Expo Go no celular, canal de homologação (link na [entrega, seção 7.1](README.md#71-onde-está-cada-coisa)), com os usuários de teste.

**Qualidade:** 582 testes automáticos na API, CI em todo PR e deploy automático da homologação a cada mudança.

## 3. Decisão sobre a publicação

Combinado: **o app não será publicado nas lojas neste semestre.** O que é entregue é o código, as contas e a documentação para o cliente publicar quando quiser.

Para publicar depois, o cliente precisa decidir:

- [ ] **Nome:** "Koin" já é marca de uma fintech brasileira (koin-docs#19)
- [ ] **Titular das contas de loja:** pessoa física ou empresa (a Apple pede D-U-N-S para empresa)
- [ ] **Quem vai manter o código:** um desenvolvedor ou equipe com acesso à organização do GitHub

## 4. Custos para operar

| Cenário | Por mês | 1º ano |
|---|---:|---:|
| 1.000 usuários ativos | R$ 248,63 | R$ 3.121,10 |
| Custo por usuário | R$ 0,25 | |

O maior custo é a leitura de faturas pela IA (US$ 0,00427 por documento, medido na homologação). Detalhes, escala e planilha editável em [custos.md](custos.md).

## 5. Entrega das contas e do código

Marcar cada item durante a reunião.

| | Item | Como entregar |
|---|---|---|
| [ ] | **Organização no GitHub** `AppFinanceiro-GECS` (koin-api, koin-app, koin-docs) | Adicionar o cliente como owner |
| [ ] | **Conta Google do produto** (`superappkoin@gmail.com`): Gemini, Google Cloud e e-mails | Passar a senha; o cliente troca a senha, a verificação em duas etapas e o e-mail de recuperação |
| [ ] | **Conta Expo** (`superappkoin2`, projeto `@superappkoin/koin`): publicação e atualizações do app | Passar a senha; o cliente troca a senha e gera um novo `EXPO_TOKEN` no GitHub |
| [ ] | **Servidor** (homologação na Oracle Cloud) | Fica no ar até **31/12/2026**, na conta do Julio. O cliente precisa de um servidor próprio antes disso (passo a passo na [entrega, seção 7.3](README.md#73-antes-de-31122026)) |
| [ ] | **Chave da IA** | A atual é provisória e sai com o servidor; o cliente cria a chave paga na conta Google do produto |
| [ ] | **Documentação** | Já está no GitHub: [entrega do projeto](README.md) |

As senhas são passadas na hora, fora de documento e de chat. Depois da troca, o time não guarda nenhuma cópia.

## 6. Próximos passos e prazos

| Quando | O quê | Quem |
|---|---|---|
| Na reunião | Entregar as contas do item 5 | Julio → cliente |
| Até 28/11/2026 | Apresentação final | Todos os grupos |
| Até 31/12/2026 | Servidor e chave da IA em nome do cliente | Cliente |
| 2027 | A VM atual é desligada | Julio |
| Quando decidir publicar | Nome, contas de loja, produção, domínio e e-mail ([entrega, seção 11](README.md#11-o-que-falta-para-a-produção)) | Cliente |

## 7. Registro da reunião

*Preencher no dia.*

- **Data:**
- **Participantes:**
- **Decisões:**
- **Contas entregues:**
- **Pendências:**
