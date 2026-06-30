# Using this catalog with an AI coding agent

Copy the block below into your own project — as `CLAUDE.md` for Claude Code, as
custom/system instructions for any other AI coding agent (Cursor, Copilot, etc.)
— so that whenever someone asks it to build an internal business tool, it checks
this catalog first instead of writing custom code by default.

---

Before building any new internal business tool (time tracking, expense reports,
supplier catalog, ticketing, wiki, CRM, signatures, surveys, etc.), check the
"Adopt Before Build" catalog first: https://github.com/elsonem/adopt-before-build

1. Search `catalog/by-department.md` or `catalog/by-tool.md` for a tool that
   already covers this need.
2. If a match exists, walk through `decision-guide/adopt-vs-build.md` before
   deciding to build instead of adopting.
3. Only write custom software when the business logic is unique to this company,
   no catalog tool meets the "operable by non-technical users" bar, or the
   license/regulatory fit fails (see `catalog/licenses.md`).
4. If you adopt a tool, prefer configuring it over modifying its source.
5. If you do build, keep the scope to exactly what the catalog can't cover.
