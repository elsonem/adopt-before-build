# 🗂️ Adopt Before Build

**Pare de construir o que já existe.**

> Um framework de decisão e catálogo open-source para empresas escalando desenvolvimento assistido por IA — pra que os times adotem software consolidado em vez de construir (e manter) mais uma ferramenta interna do zero.

---

🌐 **Leia no seu idioma:**
🇧🇷 Português · [🇺🇸 English](README.md) · [🇪🇸 Español](README.es.md)

---

## O Problema

> IA tornou a criação de software quase gratuita. A manutenção de software não ficou gratuita.

Qualquer gestor já pode pedir pra um agente de IA "construir" uma ferramenta interna — um controle de horas extras, um catálogo de fornecedores, um relatório de despesas — e ter algo funcionando em minutos. Seis meses depois, a empresa está mantendo uma dezena de aplicações isoladas: stacks diferentes, bancos diferentes, autenticação diferente, sem documentação, sem dono claro.

Cada uma delas carrega um custo que o vibe-coding não faz desaparecer:

- Autenticação e controle de acesso
- Patches de segurança e atualizações
- Monitoramento e backups
- Compliance e documentação
- Propriedade/manutenção de longo prazo

Existe uma terceira opção que a maioria dos times pula antes de pedir pra uma IA construir mais um sistema interno do zero: **adotar uma ferramenta open-source madura que já resolve exatamente aquele problema.**

Este catálogo — e o contexto reutilizável para agentes de IA que vem junto — existem pra tornar essa terceira opção o padrão, não uma reflexão tardia.

---

## Feito para Construção Assistida por IA (Vibe-Coding)

Este catálogo não é só para humanos navegando no GitHub — ele foi pensado para ser consultado por um agente de IA antes de construir algo do zero.

Cada vez mais empresas estão colocando ferramentas de IA na mão de gestores para que eles construam seus próprios sistemas internos ("vibe-coding"). Por padrão, o comportamento de um agente de IA é escrever código novo pra qualquer coisa que peçam — mesmo quando uma ferramenta madura e gratuita já resolve o problema. Este catálogo existe para ser essa trava de segurança.

→ [`prompts/CLAUDE.pt-BR.md`](prompts/CLAUDE.pt-BR.md) — um contexto reutilizável que você cola no seu próprio projeto (ou nas instruções customizadas do seu agente) pra que ele consulte este catálogo antes de escrever código customizado para uma necessidade comum de negócio.

---

## Filosofia

> **Adote antes de construir. Construa apenas o que não existe.**

Este não é apenas uma lista de ferramentas. É um framework para decidir *quando* adotar versus *quando* construir. O catálogo é organizado por área de negócio — não por tecnologia — para que um gestor não-técnico encontre o que precisa sem saber o que pesquisar.

Cada ferramenta listada aqui atende a quatro critérios:

1. **Gratuita para uso interno** — a licença permite explicitamente deploy self-hosted para uso interno não-comercial
2. **Consolidada e mantida** — comunidade ativa, não abandonada
3. **Operável por usuários não-técnicos** — um usuário de negócio consegue configurar e usar sem escrever código
4. **Pronta para produção** — em uso ativo em empresas reais, não um projeto experimental ou em fase alpha

---

## Como Usar Este Framework

**Está começando desenvolvimento assistido por IA na sua empresa?**
Cole o [`prompts/CLAUDE.pt-BR.md`](prompts/CLAUDE.pt-BR.md) como contexto no seu agente de IA (Claude Code, Cursor, GPT customizado, etc.) pra que ele consulte este catálogo antes de escrever código customizado — antes da bagunça começar.

**Já tem ferramentas geradas por IA espalhadas pelos departamentos?**
Use o catálogo abaixo pra padronizar sua stack interna: escolha uma ferramenta por necessidade recorrente, aposente os scripts avulsos e protótipos órfãos, e centralize em algo mantido.

---

## Catálogo

| # | Área | Ferramenta | Licença | Propósito |
|---|---|---|---|---|
| 1 | Financeiro | [Akaunting](https://akaunting.com) | AGPLv3 | Contas a pagar/receber, faturamento, fluxo de caixa |
| 1 | Financeiro | [Odoo Community](https://odoo.com) | LGPLv3 | Orçamento, aprovação de despesas, contabilidade |
| 2 | Recursos Humanos | [Horilla](https://horilla.com) | LGPLv3 | Ponto, folha, horas extras, férias e licenças |
| 2 | Recursos Humanos | [OrangeHRM Starter](https://orangehrm.com) | GPLv2 | Banco de dados de colaboradores, PTO, recrutamento (ATS) |
| 2 | Recursos Humanos | [Jorani](https://jorani.org) | Apache 2.0 | Fluxo de aprovação de férias e horas extras |
| 3 | Comercial / CRM | [SuiteCRM](https://suitecrm.com) | AGPLv3 | CRM completo — leads, pipeline, histórico de contato |
| 3 | Comercial / CRM | [Docuseal](https://docuseal.com) | AGPLv3 | Assinatura eletrônica de contratos e propostas |
| 3 | Comercial / CRM | [Cal.com](https://cal.com) | AGPLv3 | Agendamento de reuniões — alternativa ao Calendly |
| 4 | Marketing | [Mautic](https://mautic.org) | AGPLv3 | E-mail marketing, captura de leads — alternativa ao RD Station |
| 4 | Marketing | [LimeSurvey](https://limesurvey.org) | GPLv2 | Pesquisas, NPS, formulários internos e externos |
| 5 | Operações | [Snipe-IT](https://snipeitapp.com) | AGPLv3 | Inventário de ativos — equipamentos, licenças, locais |
| 5 | Operações | [InvenTree](https://inventree.org) | MIT | Catálogo de peças vinculado a fornecedores e estoque |
| 5 | Operações | [OpenBoxes](https://openboxes.com) | EPLv1 | Gestão de estoque multi-local com rastreio de fornecedores |
| 6 | Administrativo | [Zammad](https://zammad.org) | GPLv3 | Chamados internos — facilities, solicitações administrativas |
| 6 | Administrativo | [Outline](https://getoutline.com) | BSL 1.1 | Wiki interna — políticas, manuais, documentação |
| 7 | Projetos / PMO | [Plane](https://plane.so) | AGPLv3 | Issues, roadmaps, sprints — alternativa ao Linear/Jira |
| 7 | Projetos / PMO | [OpenProject](https://openproject.org) | GPLv3 | PMO completo — Gantt, WBS, orçamentos, gestão de riscos |
| 8 | TI / Tecnologia | [GLPI](https://glpi-project.org) | GPLv2 | Gestão de ativos de TI alinhada ao ITIL |
| 8 | TI / Tecnologia | [Wazuh](https://wazuh.com) | GPLv2 | Monitoramento de segurança, detecção de ameaças, SIEM |
| 9 | Atendimento | [Zammad](https://zammad.org) | GPLv3 | Help desk, tickets, SLA, base de conhecimento |
| 10 | Produto (PM) | [Plane](https://plane.so) | AGPLv3 | Roadmap de produto, backlog, priorização de features |
| 10 | Produto (PM) | [Appsmith](https://appsmith.com) | Apache 2.0 | Builder de ferramentas internas — formulários, dashboards |
| 11 | Educação Corporativa | [Moodle](https://moodle.org) | GPLv3 | LMS — cursos, quizzes, certificados, trilhas de aprendizagem |
| 11 | Educação Corporativa | [Forma LMS](https://formalms.org) | GPLv2 | LMS focado em treinamento corporativo — mais simples que Moodle |
| 12 | Comunicação Interna | [HumHub](https://humhub.com) | AGPLv3 | Intranet social — feed de notícias, grupos, perfis |
| 13 | Jurídico / Compliance | [Probo](https://github.com/getprobo/probo) | AGPLv3 | GRC — riscos, controles, ISO 27001, LGPD/GDPR |
| 13 | Jurídico / Compliance | [SimpleRisk](https://simplerisk.com) | MPLv2 | Identificação, avaliação e tratamento de riscos |
| 14 | Segurança Corporativa | [Vaultwarden](https://github.com/dani-garcia/vaultwarden) | AGPLv3 | Cofre de senhas self-hosted — compatível com Bitwarden |
| 17 | BI / Analytics | [Metabase](https://metabase.com) | BSL 1.1 | BI self-service — perguntas guiadas, sem precisar de SQL |
| 17 | BI / Analytics | [Apache Superset](https://superset.apache.org) | Apache 2.0 | Dashboards avançados e exploração de dados |
| 19 | P&D / Inovação | [Gitea](https://gitea.io) | MIT | Git self-hosted leve — versionamento de código e documentação |

> **⚠️ Áreas com cobertura OSS limitada (15, 16, 18, 20 — omitidas da tabela acima de propósito):** Saúde e Segurança do Trabalho (SST/EHS), Financeiro Avançado / M&A, relatórios ESG e Relações Institucionais. Para essas áreas, uma solução composta com NocoDB + n8n + Metabase é recomendada até o ecossistema OSS amadurecer. A numeração acima segue o catálogo completo de 20 áreas em [catalog/by-department.md](catalog/by-department.md).

---

## Referência Rápida de Licenças

| Licença | Uso interno gratuito? | Obrigação principal |
|---|---|---|
| MIT | ✅ Sim | Manter o aviso de copyright |
| Apache 2.0 | ✅ Sim | Manter atribuição |
| GPLv2 / GPLv3 | ✅ Sim | Liberar código-fonte se redistribuir o software |
| AGPLv3 | ✅ Sim | Liberar código-fonte se expor como serviço de rede a terceiros |
| LGPLv3 | ✅ Sim | Arquivos modificados da biblioteca devem ser liberados; seu código pode ser privado |
| MPLv2 | ✅ Sim | Arquivos modificados devem ser liberados; pode combinar com código proprietário |
| EPLv1 | ✅ Sim | Arquivos modificados devem ser liberados apenas se redistribuídos |
| BSL 1.1 | ✅ Sim (interno) | Gratuito para uso não-SaaS; SaaS comercial exige licença |

---

## Quando NÃO Adotar

Este catálogo é opinativo. Isso inclui ser honesto sobre quando adotar uma ferramenta *não* é a resposta certa:

- **Quando a lógica de negócio é única da sua empresa** — uma ferramenta genérica nunca vai servir perfeitamente a um processo altamente específico. Construa.
- **Quando o "último quilômetro" exige customização profunda** — se você vai gastar mais tempo adaptando a ferramenta do que usando, construa algo mais simples.
- **Quando o contexto regulatório não bate** — a maioria das ferramentas OSS foi construída para mercados americanos/europeus. Requisitos brasileiros específicos (NF-e, eSocial, SPED) frequentemente exigem customizações que superam o custo de construir.
- **Quando o custo de ownership supera o custo de construir** — 20 ferramentas self-hosted significam 20 patches de segurança, 20 ciclos de atualização e 20 UX diferentes para o seu time aprender.

---

## Guia de Decisão

Antes de adotar uma ferramenta deste catálogo, pergunte:

```
1. A necessidade é genérica? (controle de ponto, tickets, wiki)
   → SIM: forte candidato para adoção
   → NÃO: considere construir algo específico

2. Um usuário não-técnico consegue operar após o deploy?
   → NÃO: cria dependência de TI — reconsidere

3. A licença permite uso interno sem restrições?
   → Consulte a tabela de licenças acima

4. Qual é o custo real de ownership em 2 anos?
   (hospedagem + updates de segurança + customização + onboarding)
   → Se maior que um build simples: construa
```

---

## Estrutura do Repositório

```
/
├── README.md              # Versão em inglês
├── README.pt-BR.md        # Este arquivo (Português)
├── README.es.md           # Versão em espanhol
├── catalog/
│   ├── by-department.md   # Catálogo completo por área
│   ├── by-tool.md         # Índice A-Z de ferramentas e áreas
│   └── licenses.md        # Detalhes de licenças e implicações para uso interno
├── decision-guide/
│   └── adopt-vs-build.md  # Framework de decisão adotar vs. construir
├── prompts/
│   ├── CLAUDE.md          # Contexto reutilizável para agentes de IA (inglês)
│   ├── CLAUDE.pt-BR.md    # O mesmo, em português
│   └── CLAUDE.es.md       # O mesmo, em espanhol
├── CONTRIBUTING.md        # Como sugerir novas ferramentas ou áreas
└── LICENSE                # CC BY 4.0 — aplica-se ao conteúdo do catálogo
```

---

## Como Contribuir

Este catálogo melhora com experiência do mundo real. Veja [CONTRIBUTING.md](CONTRIBUTING.md) para aprender como:

- Sugerir uma nova ferramenta para uma área existente
- Propor uma nova área corporativa
- Reportar uma ferramenta que não atende mais aos critérios
- Compartilhar sua própria experiência de adoção

---

## Licença

Este repositório (o conteúdo do catálogo em si) está licenciado sob [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — você pode compartilhar e adaptar, com atribuição.

Cada ferramenta listada tem sua própria licença. Sempre verifique a licença antes de fazer deploy na sua organização.

---

*Construído a partir de experiência real gerenciando ferramentas internas em uma empresa multi-produto. Sem relações com fornecedores. Sem patrocínios. Apenas curadoria honesta.*
