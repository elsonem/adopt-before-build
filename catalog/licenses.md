# License Reference for Internal Use

> This guide explains each license used in the catalog from a practical perspective:
> **what you can do, what you must do, and what to watch out for** when deploying internally.
>
> This is not legal advice. When in doubt, consult your legal team.

---

## Quick Reference

| License | Free internal use | Modify | Must release source? | SaaS restriction |
|---|---|---|---|---|
| MIT | ✅ | ✅ | ❌ | ❌ |
| Apache 2.0 | ✅ | ✅ | ❌ | ❌ |
| BSD | ✅ | ✅ | ❌ | ❌ |
| GPLv2 | ✅ | ✅ | Only if you distribute | ❌ |
| GPLv3 | ✅ | ✅ | Only if you distribute | ❌ |
| LGPLv3 | ✅ | ✅ | Modified library files only | ❌ |
| AGPLv3 | ✅ | ✅ | If network-accessible to others | ✅ triggers on SaaS |
| MPLv2 | ✅ | ✅ | Modified files only | ❌ |
| EPLv1 | ✅ | ✅ | Modified files only | ❌ |
| BSL 1.1 | ✅ (internal) | ✅ | ❌ | ✅ requires commercial license |
| YetiForce PL | ✅ (internal) | ✅ | ❌ | ✅ no resale/SaaS |

---

## Detailed Explanations

### MIT
**The most permissive license.** You can do almost anything — use, copy, modify, merge, publish, distribute, sublicense, or sell — as long as you include the original copyright notice.

**For internal use:** Zero restrictions. Deploy, modify, and integrate freely.

**Watch out for:** Nothing significant for internal use.

**Tools:** InvenTree, Gitea

---

### Apache 2.0
Similar to MIT but with an explicit patent grant — contributors cannot later sue you for patent infringement over the code they contributed.

**For internal use:** Zero restrictions. Deploy, modify, and integrate freely.

**Watch out for:** If you distribute the software externally, you must include attribution and the license text.

**Tools:** Appsmith, Apache Superset, Jorani

---

### BSD
A permissive license very similar to MIT — use, modify, and distribute freely as long as you keep the copyright notice. The 2-clause and 3-clause variants differ only in a non-endorsement clause (3-clause forbids using contributor names to promote derived products).

**For internal use:** Zero restrictions. Deploy, modify, and integrate freely.

**Watch out for:** Nothing significant for internal use.

**Tools:** Redash

---

### GPLv2 and GPLv3
The "copyleft" licenses. The key rule: **if you distribute the software** (give it to someone outside your organization), you must also distribute the source code under the same license.

**For internal use:** No restriction at all. You can modify, self-host, and use internally without ever releasing your changes — because you are not distributing it.

**GPLv3 adds:** Protection against "tivoization" (hardware that runs GPL software but prevents modification) and better patent protections.

**Watch out for:** If your company *sells* or *distributes* a modified version externally, the source must be released. Internal use only = no obligation.

**Tools:** GLPI, Wazuh, OrangeHRM, LimeSurvey, Moodle, Forma LMS, OpenProject, Zammad, Chamilo, Budibase, UVDesk

---

### LGPLv3
A "weaker" copyleft designed for libraries. The rule: **if you modify the LGPL library itself**, you must release those modifications. But if you just *use* the library in your own application, your application can remain proprietary.

**For internal use:** No restriction. Deploy and use freely.

**Watch out for:** If you fork and modify Odoo or Horilla themselves (not just configure them), those modifications technically should be released. Configuration and customization via the UI is not modification of the library.

**Tools:** Odoo Community, Horilla

---

### AGPLv3
GPL with an important addition: the "network use" clause. Normally, running software on a server for internal users counts as internal use (no distribution = no obligation). AGPL closes this "loophole": **if you make the software accessible over a network to users outside your organization**, you must release the source.

**For internal use:** No restriction. Your employees using an AGPLv3 tool internally does not trigger any obligation.

**Watch out for:** If you expose an AGPLv3 tool to external users (customers, partners, public) as a service, you must release the source — or negotiate a commercial license with the vendor.

**Tools:** Akaunting, SuiteCRM, Cal.com, Mautic, Snipe-IT, Plane, Vikunja, Probo, HumHub, NocoDB, n8n, Vaultwarden, Grafana

---

### MPLv2
File-level copyleft. Only the files you modify must be released under MPL. You can combine MPL code with proprietary code in the same project.

**For internal use:** No restriction.

**Watch out for:** If you modify MPL-licensed files and distribute them, release those specific files under MPL.

**Tools:** SimpleRisk

---

### EPLv1
Similar to MPL — file-level copyleft. Modifications to EPL files must be released if distributed.

**For internal use:** No restriction.

**Tools:** OpenBoxes

---

### BSL 1.1 (Business Source License)
A "source available" license, not technically OSI-approved open source. The key rule: **free for any use that is not "production use" in a competing product or paid SaaS offering**.

Metabase and Outline use BSL 1.1 with this specific condition: you cannot use the software to offer it as a service to external paying customers. Internal use — including by a company of any size — is explicitly free.

**For internal use:** Free, unconditionally.

**Watch out for:** If your company's business model involves offering Metabase or Outline as a hosted service to external customers, you need a commercial license.

**Tools:** Metabase, Outline

---

### YetiForce Public License
A custom license created by the YetiForce team. Key points:
- Free to use and modify for internal company purposes
- Cannot be resold or offered as a SaaS to third parties
- Cannot be rebranded and distributed

**For internal use:** Free.

**Watch out for:** Less legal certainty than standard licenses (MIT, GPL, Apache). If your legal team requires a standard SPDX license, use SuiteCRM (AGPLv3) instead.

**Tools:** YetiForce CRM

---

## Common Scenarios

### "We want to self-host Metabase for our finance team."
✅ Allowed under BSL 1.1. Internal use has no restriction.

### "We want to modify Zammad to add a custom field."
✅ Allowed. GPLv3 only requires source release if you *distribute* the modified software. Internal modifications stay private.

### "We want to expose our n8n instance so customers can trigger automations."
⚠️ Review carefully. AGPLv3 requires source release if you make the software network-accessible to users outside your organization. If customers interact with n8n directly, you are distributing via network. Either release the source or obtain a commercial license from n8n GmbH.

### "We want to build a SaaS product on top of Appsmith."
✅ Apache 2.0 has no SaaS restriction. You can build and commercialize freely.

### "We want to resell a customized version of YetiForce."
❌ Not allowed under YetiForce PL. Use SuiteCRM (AGPLv3) with a commercial license negotiation if you need to distribute.

---

*Last updated: 2026. License terms can change with new versions — always verify against the official repository.*
