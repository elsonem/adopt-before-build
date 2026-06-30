# Adopt vs. Build — Decision Guide

> The central question this catalog tries to answer is not "which tool should I use?"
> It is: **should I adopt an existing tool, or build something specific?**
>
> This guide gives you a framework to answer that question honestly — including when the answer is "build."

---

## The Core Principle

> **Adopt when the problem is generic. Build when the problem is yours.**

Most internal business needs are not unique. Time tracking, document signing, survey collection, asset inventory — these problems have been solved thousands of times. Using a proven tool is almost always faster, cheaper, and more reliable than building a custom solution.

But "almost always" is not "always." There are real situations where building is the right answer.

---

## The Decision Flowchart

```
Start here: Someone needs an internal tool.
│
├─► Is the need clearly generic?
│   (time tracking, ticketing, wiki, invoicing, surveys...)
│   │
│   ├─► YES → Check the catalog → Strong adoption candidate
│   │
│   └─► NO → Is it mostly generic with a few custom rules?
│             │
│             ├─► YES → Adopt + configure. Avoid modifying source code.
│             │
│             └─► NO → The logic is unique to your company → BUILD
│
├─► Can a non-technical user operate it after deploy?
│   │
│   ├─► YES → Continue evaluation
│   │
│   └─► NO → Creates IT dependency every time someone needs a change
│             → Reconsider, or ensure IT ownership is budgeted
│
├─► Does the license allow internal use?
│   │
│   ├─► YES → Continue evaluation (see license guide)
│   │
│   └─► UNCLEAR → Check catalog/licenses.md before proceeding
│
├─► What is the real ownership cost over 2 years?
│   Consider:
│   - Hosting and infrastructure
│   - Security patches and version updates
│   - Customization to fit your specific process
│   - Onboarding team members to a new UI
│   - What happens when the tool is abandoned or relicensed
│   │
│   ├─► Lower than building → ADOPT
│   │
│   └─► Higher than building → BUILD something simpler and specific
│
└─► Does the regulatory/legal context match?
    │
    ├─► YES → ADOPT
    │
    └─► NO → Local tax rules, labor laws, specific compliance requirements
              that the tool doesn't support and can't be configured to support
              → BUILD or seek a local vendor
```

---

## When to Adopt

✅ The need is clearly generic — it exists in any company regardless of industry or size

✅ A non-technical user will be the primary operator, not IT

✅ The tool is actively maintained (last release < 12 months)

✅ Customization is possible via UI/configuration, not source code changes

✅ Onboarding a new team member to the tool takes hours, not days

✅ The tool has been deployed in organizations similar to yours

---

## When to Build

🔨 The business logic is specific to your company or industry and has no generic equivalent

🔨 The "last mile" customization would cost more than building something simple from scratch

🔨 Local regulatory requirements (tax rules, labor laws, compliance standards) are not supported and cannot be configured

🔨 The tool requires IT intervention every time a business user needs a change — ownership never leaves IT

🔨 The total ownership cost over 2 years exceeds a simple custom build

🔨 The tool solves 80% of the problem but the missing 20% is the critical part

---

## The Hidden Costs of Adoption

Adopting is not free. These costs are often invisible until it's too late:

| Cost | Description |
|---|---|
| **Deploy complexity** | Someone has to set up Docker, configure the database, set up SSO, configure SMTP, set permissions. This is IT work. |
| **Security maintenance** | Every self-hosted tool is a CVE waiting to happen. Someone must monitor releases and apply patches. |
| **UX fragmentation** | 10 tools = 10 different interfaces. Cognitive overhead adds up across teams. |
| **Customization debt** | Small tweaks to fit your process accumulate. At some point you own a fork, not a tool. |
| **Abandonment risk** | Open-source projects die. Relicensing happens (HashiCorp → BSL, Elasticsearch → SSPL). Always have an exit plan. |
| **Token cost is not zero** | If users need Claude Code to customize the tool repeatedly, the "token savings" argument weakens. |

---

## The Hidden Costs of Building

Building is not free either. These costs are often underestimated:

| Cost | Description |
|---|---|
| **Consistency** | Every developer / vibe-coder builds differently. Without standards, you end up with 10 tools that look like 10 different products. |
| **Maintenance** | Custom code has bugs. Someone has to fix them. The original builder may not be available. |
| **Feature creep** | Once you build, requests come. "Can you add X?" never stops. |
| **Security** | A self-built internal tool with no security review is a liability. |
| **Documentation** | Undocumented tools become black boxes when the builder leaves. |

---

## The Composable Middle Ground

Many situations don't require a full tool adoption or a full custom build. A **composed solution** using two or three general-purpose tools is often the right answer:

| Need | Composed solution |
|---|---|
| Custom ESG tracker | NocoDB (database) + Metabase (dashboards) + n8n (alerts) |
| Simple vendor register | NocoDB alone |
| Approval workflow | n8n + Outline (for policy documentation) |
| M&A deal pipeline | Plane (issues) + NocoDB (data) + Metabase (reports) |
| SST incident register | NocoDB + n8n (deadline alerts) |

The composed approach works best when:
- The domain has no mature OSS tool
- The need is genuinely simple (a database + some automation)
- The team can maintain the composition without constant IT support

---

## A Note on AI-Assisted Building (Vibe-Coding)

The rise of AI-assisted development (Claude Code, Cursor, Copilot) changes the build vs. adopt equation in one important way: **the cost of building simple tools is lower than it used to be.**

This does not mean "always build." It means:

- The threshold for "build" is lower for simple, well-defined needs
- The threshold for "adopt" is unchanged for complex domains (HR, finance, security)
- The risk of over-building increases — AI makes it easy to build things that didn't need to exist

A good rule of thumb: **if a non-technical user can describe what they need in two sentences, it's a build candidate. If they need a paragraph, it's an adopt candidate.**

---

## Summary Table

| Signal | Adopt | Build | Composed |
|---|---|---|---|
| Generic domain | ✅ | | |
| Unique business logic | | ✅ | |
| Partially generic | | | ✅ |
| Non-technical operator | ✅ | | |
| IT-dependent operation | | ✅ | |
| Low ownership cost | ✅ | | |
| High customization needed | | ✅ | |
| No mature OSS exists | | | ✅ |
| Regulatory mismatch | | ✅ | |
| Simple + well-defined need | | ✅ | |
| Complex domain | ✅ | | |
