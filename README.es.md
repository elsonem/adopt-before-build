# 🗂️ Adopt Before Build

**Deja de construir lo que ya existe.**

> Un framework de decisión y catálogo open-source para empresas escalando desarrollo asistido por IA — para que los equipos adopten software consolidado en lugar de construir (y mantener) una herramienta interna más desde cero.

---

🌐 **Lee en tu idioma:**
[🇧🇷 Português](README.md) · [🇺🇸 English](README.en.md) · 🇪🇸 Español

---

## El Problema

> La IA hizo que crear software fuera casi gratis. Mantener software no se volvió gratis.

Cualquier gestor ya puede pedirle a un agente de IA que "construya" una herramienta interna — un control de horas extra, un catálogo de proveedores, un informe de gastos — y tener algo funcionando en minutos. Seis meses después, la empresa mantiene una docena de aplicaciones aisladas: stacks diferentes, bases de datos diferentes, autenticación diferente, sin documentación, sin dueño claro.

Cada una de ellas tiene un costo que el vibe-coding no hace desaparecer:

- Autenticación y control de acceso
- Parches de seguridad y actualizaciones
- Monitoreo y backups
- Compliance y documentación
- Propiedad y mantenimiento a largo plazo

Existe una tercera opción que la mayoría de los equipos se salta antes de pedirle a una IA que construya otro sistema interno desde cero: **adoptar una herramienta open-source madura que ya resuelve exactamente ese problema.**

Este catálogo — y el contexto reutilizable para agentes de IA que lo acompaña — existen para hacer que esa tercera opción sea la opción por defecto, no una idea de último momento.

---

## Diseñado para Construcción Asistida por IA (Vibe-Coding)

Este catálogo no es solo para humanos navegando en GitHub — está pensado para ser consultado por un agente de IA antes de construir algo desde cero.

Cada vez más empresas ponen herramientas de IA en manos de gestores para que construyan sus propios sistemas internos ("vibe-coding"). Por defecto, el comportamiento de un agente de IA es escribir código nuevo para lo que sea que le pidan — incluso cuando una herramienta madura y gratuita ya resuelve el problema. Este catálogo existe para ser esa salvaguarda.

→ [`prompts/CLAUDE.es.md`](prompts/CLAUDE.es.md) — un contexto reutilizable que copias en tu propio proyecto (o en las instrucciones personalizadas de tu agente) para que consulte este catálogo antes de escribir código personalizado para una necesidad común de negocio.

---

## Filosofía

> **Adopta antes de construir. Construye solo lo que no existe.**

Esto no es solo una lista de herramientas. Es un framework para decidir *cuándo* adoptar versus *cuándo* construir. El catálogo está organizado por área de negocio — no por tecnología — para que un gestor no técnico pueda encontrar lo que necesita sin saber qué buscar.

Cada herramienta listada aquí cumple cuatro criterios:

1. **Gratuita para uso interno** — la licencia permite explícitamente el despliegue self-hosted para uso interno no comercial
2. **Consolidada y mantenida** — comunidad activa, no abandonada
3. **Operable por usuarios no técnicos** — un usuario de negocio puede configurarla y usarla sin escribir código
4. **Lista para producción** — en uso activo en empresas reales, no un proyecto experimental o en fase alpha

---

## Cómo Usar Este Framework

**¿Estás empezando con desarrollo asistido por IA en tu empresa?**
Pon el [`prompts/CLAUDE.es.md`](prompts/CLAUDE.es.md) como contexto en tu agente de IA (Claude Code, Cursor, GPT personalizado, etc.) para que consulte este catálogo antes de escribir código personalizado — antes de que empiece el desorden.

**¿Ya tienes herramientas generadas por IA dispersas entre departamentos?**
Usa el catálogo de abajo para estandarizar tu stack interno: elige una herramienta por necesidad recurrente, retira los scripts sueltos y prototipos huérfanos, y centraliza en algo mantenido.

---

## Catálogo

| # | Área | Herramienta | Licencia | Propósito |
|---|---|---|---|---|
| 1 | Finanzas | [Akaunting](https://akaunting.com) | AGPLv3 | Cuentas por pagar/cobrar, facturación, flujo de caja |
| 1 | Finanzas | [Odoo Community](https://odoo.com) | LGPLv3 | Presupuesto, aprobación de gastos, contabilidad |
| 2 | Recursos Humanos | [Horilla](https://horilla.com) | LGPLv3 | Control de tiempo, nómina, horas extra, vacaciones |
| 2 | Recursos Humanos | [OrangeHRM Starter](https://orangehrm.com) | GPLv2 | Base de datos de empleados, PTO, reclutamiento (ATS) |
| 2 | Recursos Humanos | [Jorani](https://jorani.org) | Apache 2.0 | Flujo de aprobación de vacaciones y horas extra |
| 3 | Ventas / CRM | [SuiteCRM](https://suitecrm.com) | AGPLv3 | CRM completo — leads, pipeline, historial de contactos |
| 3 | Ventas / CRM | [Docuseal](https://docuseal.com) | AGPLv3 | Firma electrónica de contratos y propuestas |
| 3 | Ventas / CRM | [Cal.com](https://cal.com) | AGPLv3 | Programación de reuniones — alternativa a Calendly |
| 4 | Marketing | [Mautic](https://mautic.org) | AGPLv3 | Email marketing, captación de leads — alternativa a HubSpot |
| 4 | Marketing | [LimeSurvey](https://limesurvey.org) | GPLv2 | Encuestas, NPS, formularios internos y externos |
| 5 | Operaciones | [Snipe-IT](https://snipeitapp.com) | AGPLv3 | Inventario de activos — equipos, licencias, ubicaciones |
| 5 | Operaciones | [InvenTree](https://inventree.org) | MIT | Catálogo de piezas vinculado a proveedores y stock |
| 5 | Operaciones | [OpenBoxes](https://openboxes.com) | EPLv1 | Gestión de stock multi-ubicación con seguimiento de proveedores |
| 6 | Administración | [Zammad](https://zammad.org) | GPLv3 | Tickets internos — facilities, solicitudes administrativas |
| 6 | Administración | [Outline](https://getoutline.com) | BSL 1.1 | Wiki interna — políticas, manuales, documentación |
| 7 | Proyectos / PMO | [Plane](https://plane.so) | AGPLv3 | Issues, roadmaps, sprints — alternativa a Linear/Jira |
| 7 | Proyectos / PMO | [OpenProject](https://openproject.org) | GPLv3 | PMO completo — Gantt, WBS, presupuestos, gestión de riesgos |
| 8 | TI / Tecnología | [GLPI](https://glpi-project.org) | GPLv2 | Gestión de activos de TI alineada con ITIL |
| 8 | TI / Tecnología | [Wazuh](https://wazuh.com) | GPLv2 | Monitoreo de seguridad, detección de amenazas, SIEM |
| 9 | Atención al Cliente | [Zammad](https://zammad.org) | GPLv3 | Help desk, tickets, SLA, base de conocimiento |
| 10 | Producto (PM) | [Plane](https://plane.so) | AGPLv3 | Roadmap de producto, backlog, priorización de features |
| 10 | Producto (PM) | [Appsmith](https://appsmith.com) | Apache 2.0 | Constructor de herramientas internas — formularios, dashboards |
| 11 | Formación (L&D) | [Moodle](https://moodle.org) | GPLv3 | LMS — cursos, cuestionarios, certificados, rutas de aprendizaje |
| 11 | Formación (L&D) | [Forma LMS](https://formalms.org) | GPLv2 | LMS enfocado en formación corporativa — más simple que Moodle |
| 12 | Comunicación Interna | [HumHub](https://humhub.com) | AGPLv3 | Intranet social — feed de noticias, grupos, perfiles |
| 13 | Legal / Compliance | [Probo](https://github.com/getprobo/probo) | AGPLv3 | GRC — riesgos, controles, ISO 27001, GDPR |
| 13 | Legal / Compliance | [SimpleRisk](https://simplerisk.com) | MPLv2 | Identificación, evaluación y tratamiento de riesgos |
| 14 | Seguridad Corporativa | [Vaultwarden](https://github.com/dani-garcia/vaultwarden) | AGPLv3 | Gestor de contraseñas self-hosted — compatible con Bitwarden |
| 17 | BI / Analytics | [Metabase](https://metabase.com) | BSL 1.1 | BI self-service — preguntas guiadas, sin necesidad de SQL |
| 17 | BI / Analytics | [Apache Superset](https://superset.apache.org) | Apache 2.0 | Dashboards avanzados y exploración de datos |
| 19 | I+D / Innovación | [Gitea](https://gitea.io) | MIT | Git self-hosted ligero — versionado de código y documentación |

> **⚠️ Áreas con cobertura OSS limitada (15, 16, 18, 20 — omitidas de la tabla anterior a propósito):** Salud y Seguridad Ocupacional (EHS/SST), Finanzas Avanzadas / M&A, reportes ESG y Asuntos Gubernamentales. Para estas áreas, se recomienda una solución compuesta con NocoDB + n8n + Metabase hasta que el ecosistema OSS madure. La numeración anterior sigue el catálogo completo de 20 áreas en [catalog/by-department.md](catalog/by-department.md).

---

## Referencia Rápida de Licencias

| Licencia | ¿Uso interno gratuito? | Obligación principal |
|---|---|---|
| MIT | ✅ Sí | Mantener el aviso de copyright |
| Apache 2.0 | ✅ Sí | Mantener atribución |
| GPLv2 / GPLv3 | ✅ Sí | Liberar código fuente si redistribuyes el software |
| AGPLv3 | ✅ Sí | Liberar código fuente si lo expones como servicio de red a terceros |
| LGPLv3 | ✅ Sí | Archivos modificados de la librería deben liberarse; tu código puede ser privado |
| MPLv2 | ✅ Sí | Archivos modificados deben liberarse; puede combinarse con código propietario |
| EPLv1 | ✅ Sí | Archivos modificados deben liberarse solo si se redistribuyen |
| BSL 1.1 | ✅ Sí (interno) | Gratuito para uso no-SaaS; SaaS comercial requiere licencia |

---

## Cuándo NO Adoptar

Este catálogo es opinativo. Eso incluye ser honesto sobre cuándo adoptar una herramienta *no* es la respuesta correcta:

- **Cuando la lógica de negocio es única de tu empresa** — una herramienta genérica nunca encajará perfectamente en un proceso altamente específico. Constrúyelo.
- **Cuando el "último kilómetro" requiere personalización profunda** — si vas a gastar más tiempo adaptando la herramienta que usándola, construye algo más simple.
- **Cuando el contexto regulatorio no coincide** — la mayoría de las herramientas OSS fueron construidas para mercados americanos/europeos. Los requisitos locales específicos frecuentemente exigen adaptaciones que superan el costo de construir.
- **Cuando el costo de ownership supera el costo de construir** — 20 herramientas self-hosted significan 20 parches de seguridad, 20 ciclos de actualización y 20 UX diferentes que tu equipo debe aprender.

---

## Guía de Decisión

Antes de adoptar una herramienta de este catálogo, pregunta:

```
1. ¿La necesidad es genérica? (control de tiempo, tickets, wiki)
   → SÍ:  candidato fuerte para adopción
   → NO:  considera construir algo específico

2. ¿Un usuario no técnico puede operarla después del despliegue?
   → NO:  crea dependencia de TI — reconsidera

3. ¿La licencia permite uso interno sin restricciones?
   → Consulta la tabla de licencias arriba

4. ¿Cuál es el costo real de ownership en 2 años?
   (hosting + actualizaciones de seguridad + personalización + onboarding)
   → Si es mayor que una construcción simple: construye
```

---

## Estructura del Repositorio

```
/
├── README.md              # Versión en portugués (predeterminada)
├── README.en.md           # Versión en inglés
├── README.es.md           # Este archivo (Español)
├── catalog/
│   ├── by-department.md   # Catálogo completo por área
│   ├── by-tool.md         # Índice A-Z de herramientas y áreas
│   └── licenses.md        # Detalles de licencias e implicaciones para uso interno
├── decision-guide/
│   └── adopt-vs-build.md  # Framework de decisión adoptar vs. construir
├── prompts/
│   ├── CLAUDE.md          # Contexto reutilizable para agentes de IA (inglés)
│   ├── CLAUDE.pt-BR.md    # Lo mismo, en portugués
│   └── CLAUDE.es.md       # Lo mismo, en español
├── CONTRIBUTING.md        # Cómo sugerir nuevas herramientas o áreas
└── LICENSE                # CC BY 4.0 — aplica al contenido del catálogo
```

---

## Cómo Contribuir

Este catálogo mejora con experiencia del mundo real. Ve [CONTRIBUTING.md](CONTRIBUTING.md) para aprender cómo:

- Sugerir una nueva herramienta para un área existente
- Proponer una nueva área corporativa
- Reportar una herramienta que ya no cumple los criterios
- Compartir tu propia experiencia de adopción

---

## Licencia

Este repositorio (el contenido del catálogo en sí) está licenciado bajo [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — puedes compartirlo y adaptarlo, con atribución.

Cada herramienta listada tiene su propia licencia. Siempre verifica la licencia antes de desplegar en tu organización.

---

*Construido desde experiencia real gestionando herramientas internas en una empresa multi-producto. Sin relaciones con proveedores. Sin patrocinios. Solo curaduría honesta.*
