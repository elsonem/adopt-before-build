# 🗂️ Adopt Before Build

**Stop building what already exists.**

> A decision framework and open-source catalog for companies scaling AI-assisted development — so teams adopt proven software instead of building (and maintaining) yet another internal tool from scratch.

---

🌐 **Read in your language:**
[🇧🇷 Português](README.md) · 🇺🇸 English · [🇪🇸 Español](README.es.md)

---

## The Problem

> AI made software creation almost free. Software maintenance didn't become free.

Any manager can now ask an AI agent to "build" an internal tool — a time-off tracker, a supplier catalog, an internal wiki — and get something working in minutes. Six months later, the company is maintaining a dozen one-off applications: different stacks, different databases, different authentication, no documentation, no clear owner.

Every one of those carries a cost vibe-coding doesn't make go away:

- Authentication and access control
- Security patches and updates
- Monitoring and backups
- Compliance and documentation
- Long-term ownership

There is a third option most teams skip before asking an AI to build yet another internal system from scratch: **adopt a mature, free, open-source tool that already solves that exact problem.**

This catalog — and the reusable AI-agent context that ships with it — exist to make that third option the default, not an afterthought.

---

## Built for AI-Assisted Building (Vibe-Coding)

This catalog isn't only for humans browsing GitHub — it's meant to be consulted by an AI coding agent before it builds something from scratch.

More companies are giving managers AI tools to build their own internal software ("vibe-coding"). Left on its own, an AI agent's default behavior is to write new code for whatever it's asked — even when a mature, free tool already solves the problem. This catalog exists to be that guardrail.

→ [`prompts/CLAUDE.md`](prompts/CLAUDE.md) — a reusable context block you drop into your own project (or your agent's custom instructions) so it checks this catalog before writing custom code for a common business need.

---

## Philosophy

> **Adopt before you build. Build only what doesn't exist.**

This is not just a list of tools. It is a framework for deciding *when* to adopt versus *when* to build. The catalog is organized by business area — not by technology — so that a non-technical manager can find what they need without knowing what to search for.

Every tool listed here meets four criteria:

1. **Free for internal use** — license explicitly allows self-hosted, non-commercial internal deployment
2. **Proven and maintained** — active community, not abandoned
3. **Operable by non-technical users** — a business user can configure and use it without writing code
4. **Production-ready** — actively deployed in real companies, not an experimental or alpha-stage project

---

## How to Use This Framework

**Starting AI-assisted development in your company?**
Drop [`prompts/CLAUDE.md`](prompts/CLAUDE.md) into your AI agent as reusable context (Claude Code, Cursor, custom GPT, etc.) so it checks this catalog before writing custom code — before the sprawl starts.

**Already have AI-generated tools scattered across departments?**
Use the catalog below to baseline your internal stack: pick one tool per recurring need, retire the one-off scripts and orphaned prototypes, and centralize on something maintained.

---

## Catalog

| # | Department | Tool | License | Purpose |
|---|---|---|---|---|
| 1 | Finance | [Akaunting](https://akaunting.com) | AGPLv3 | Accounts payable/receivable, invoicing, cash flow |
| 1 | Finance | [Odoo Community](https://odoo.com) | LGPLv3 | Budget planning, expense management, accounting |
| 2 | Human Resources | [Horilla](https://horilla.com) | LGPLv3 | Time tracking, payroll, overtime, leave management |
| 2 | Human Resources | [OrangeHRM Starter](https://orangehrm.com) | GPLv2 | Employee database, PTO, recruitment (ATS) |
| 2 | Human Resources | [Jorani](https://jorani.org) | Apache 2.0 | Leave and overtime approval workflows |
| 3 | Sales / CRM | [SuiteCRM](https://suitecrm.com) | AGPLv3 | Full CRM — leads, pipeline, contact history |
| 3 | Sales / CRM | [Docuseal](https://docuseal.com) | AGPLv3 | Electronic signature for contracts and proposals |
| 3 | Sales / CRM | [Cal.com](https://cal.com) | AGPLv3 | Meeting scheduling — Calendly alternative |
| 4 | Marketing | [Mautic](https://mautic.org) | AGPLv3 | Email marketing, lead capture — HubSpot alternative |
| 4 | Marketing | [LimeSurvey](https://limesurvey.org) | GPLv2 | Surveys, NPS, internal feedback forms |
| 5 | Operations | [Snipe-IT](https://snipeitapp.com) | AGPLv3 | Asset inventory — equipment, licenses, locations |
| 5 | Operations | [InvenTree](https://inventree.org) | MIT | Parts catalog linked to suppliers and stock levels |
| 5 | Operations | [OpenBoxes](https://openboxes.com) | EPLv1 | Multi-location stock management with supplier tracking |
| 6 | Administration | [Zammad](https://zammad.org) | GPLv3 | Internal ticketing — facilities, admin requests |
| 6 | Administration | [Outline](https://getoutline.com) | BSL 1.1 | Company wiki — policies, manuals, documentation |
| 7 | Project Management | [Plane](https://plane.so) | AGPLv3 | Issues, roadmaps, sprints — Linear/Jira alternative |
| 7 | Project Management | [OpenProject](https://openproject.org) | GPLv3 | Full PMO — Gantt, WBS, budgets, risk management |
| 8 | IT / Technology | [GLPI](https://glpi-project.org) | GPLv2 | IT asset management aligned with ITIL |
| 8 | IT / Technology | [Wazuh](https://wazuh.com) | GPLv2 | Security monitoring, threat detection, SIEM |
| 9 | Customer Support | [Zammad](https://zammad.org) | GPLv3 | Help desk, tickets, SLA, knowledge base |
| 10 | Product Management | [Plane](https://plane.so) | AGPLv3 | Product roadmap, backlog, feature prioritization |
| 10 | Product Management | [Appsmith](https://appsmith.com) | Apache 2.0 | Internal tools builder — forms, dashboards, admin panels |
| 11 | Training & Dev (L&D) | [Moodle](https://moodle.org) | GPLv3 | LMS — courses, quizzes, certificates, learning paths |
| 11 | Training & Dev (L&D) | [Forma LMS](https://formalms.org) | GPLv2 | Corporate-focused LMS — simpler than Moodle |
| 12 | Internal Comms | [HumHub](https://humhub.com) | AGPLv3 | Internal social intranet — news feed, groups, profiles |
| 13 | Legal / Compliance | [Probo](https://github.com/getprobo/probo) | AGPLv3 | GRC — risk, controls, ISO 27001, GDPR/LGPD |
| 13 | Legal / Compliance | [SimpleRisk](https://simplerisk.com) | MPLv2 | Risk identification, assessment, and treatment |
| 14 | Corporate Security | [Vaultwarden](https://github.com/dani-garcia/vaultwarden) | AGPLv3 | Self-hosted password manager — Bitwarden compatible |
| 17 | BI / Analytics | [Metabase](https://metabase.com) | BSL 1.1 | Self-service BI — guided questions, no SQL required |
| 17 | BI / Analytics | [Apache Superset](https://superset.apache.org) | Apache 2.0 | Advanced dashboards and data exploration |
| 19 | R&D / Innovation | [Gitea](https://gitea.io) | MIT | Lightweight self-hosted Git — code and docs versioning |

> **⚠️ Areas with limited OSS coverage (15, 16, 18, 20 — intentionally omitted from the table above):** Occupational Health & Safety (SST/EHS), Advanced Finance / M&A, ESG reporting, and Government Affairs. For these, a composed approach using NocoDB + n8n + Metabase is recommended until the OSS ecosystem matures. The numbering above follows the full 20-area catalog in [catalog/by-department.md](catalog/by-department.md).

---

## License Quick Reference

| License | Free for internal use? | Key obligation |
|---|---|---|
| MIT | ✅ Yes | Keep copyright notice |
| Apache 2.0 | ✅ Yes | Keep attribution |
| GPLv2 / GPLv3 | ✅ Yes | Distribute source if you redistribute the software |
| AGPLv3 | ✅ Yes | Distribute source if you expose it as a network service to others |
| LGPLv3 | ✅ Yes | Modified library files must be released; your own code can stay private |
| MPLv2 | ✅ Yes | Modified files must be released; can combine with proprietary code |
| EPLv1 | ✅ Yes | Modified files must be released only if you redistribute them |
| BSL 1.1 | ✅ Yes (internal) | Free for any non-SaaS use; commercial SaaS requires a license |

---

## When NOT to Adopt

This catalog is opinionated. That includes being honest about when adopting a tool is *not* the right answer:

- **When the business logic is unique to your company** — a tool built for generic use will never fit a highly specific workflow. Build it.
- **When the "last mile" requires deep customization** — if you'll spend more time adapting the tool than using it, build something simpler.
- **When the regulatory context doesn't match** — most OSS tools were built for US/EU markets. Brazilian-specific requirements (NF-e, eSocial, SPED) often require customization that exceeds the cost of building.
- **When the ownership cost is higher than the build cost** — 20 self-hosted tools means 20 security patches, 20 update cycles, 20 different UX experiences for your team.

---

## Decision Guide

Before adopting a tool from this catalog, ask:

```
1. Is the need generic (time tracking, ticketing, wiki)?
   → YES: strong candidate for adoption
   → NO:  consider building something specific

2. Will a non-technical user be able to operate it after deploy?
   → NO:  it creates IT dependency — reconsider

3. Does the license allow internal use without restrictions?
   → Check the license table above

4. What is the real ownership cost over 2 years?
   (hosting + security updates + customization + onboarding)
   → If higher than a simple build: build
```

---

## Repository Structure

```
/
├── README.md              # Portuguese version (default)
├── README.en.md           # This file (English)
├── README.es.md           # Spanish version
├── catalog/
│   ├── by-department.md   # Full catalog organized by department
│   ├── by-tool.md         # A-Z index of all tools with areas served
│   └── licenses.md        # License details and internal-use implications
├── decision-guide/
│   └── adopt-vs-build.md  # Framework for the build vs. adopt decision
├── prompts/
│   ├── CLAUDE.md          # Reusable context block for AI coding agents (English)
│   ├── CLAUDE.pt-BR.md    # Same, in Portuguese
│   └── CLAUDE.es.md       # Same, in Spanish
├── CONTRIBUTING.md        # How to suggest new tools or areas
└── LICENSE                # CC BY 4.0 — applies to catalog content
```

---

## Contributing

This catalog improves with real-world experience. See [CONTRIBUTING.md](CONTRIBUTING.md) to learn how to:

- Suggest a new tool for an existing area
- Propose a new corporate area
- Report a tool that no longer meets the criteria
- Share your own adoption experience

---

## License

This repository (the catalog content itself) is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — you are free to share and adapt it, with attribution.

Each tool listed has its own license. Always verify the license before deploying in your organization.

---

*Built from real-world experience managing internal tools across a multi-product company. No vendor relationships. No sponsorships. Just honest curation.*
