# Kong Portal Saves

Git-backed drafts and copies of **Bankrate Konnect Developer Portal** pages and snippets. Content is written in **MDC** (Markdown with Kong block components), not plain HTML.

The **live site** (routes, visibility, theme, global nav, layout snippets) lives in **Konnect**. This repo is where you **author, review, and version** page bodies and snippet definitions before syncing them into the portal.

## Official reference

- [Konnect Developer Portal documentation](https://portaldocs.konghq.com/) — Markdown & MDC, components, snippets, layouts.
- [Markdown & MDC syntax](https://portaldocs.konghq.com/getting-started/markdown) — `::` block components, YAML props, slots (`#slotName`), nesting.

## Repository layout

| Area | Purpose |
|------|--------|
| Repo root (e.g. `getting-started`, `api-key-guide`, `bankrate-content-feeds`) | Full page documents: YAML frontmatter + MDC body. Filenames are local labels; **published URLs are set in Konnect** (slug). |
| `Snippets/` | Reusable snippet bodies referenced from pages with `::snippet` / `:::snippet`. Snippet `name:` must match what is configured in Konnect. |
| `images/` | Static assets (screenshots, icons). Pages may reference GitHub raw URLs or portal static paths—confirm images resolve in Konnect if you change hosting. |
| `Kong-Component-Library.md` | In-repo examples and notes aligned with Kong’s component docs—useful when choosing props and patterns. |
| `Kong-style-overrides.css` | CSS reference/overrides used with the portal theme (as applicable to your Konnect setup). |

## Typical page structure

Most guide-style pages follow this pattern:

1. **YAML frontmatter** — `title`, `description`, and `page-layout` (e.g. `sidebar-left: "example-guides-page-nav"`, `sidebar-right: "example-page-toc"`). Layout snippet names must exist in your Konnect project.
2. **`::page-hero`** — Tagline, title, description slots.
3. **`::page-section`** — Main prose: `##` / `###` headings, tables, fenced code, nested components (`::alert`, `::image`, etc.).

Many HTML comments in pages say **sync body to Konnect** and suggest example slugs (e.g. `/guides/bankrate-content-feeds`). Treat those as the handoff step, not automatic deploy.

## Workflow (short)

1. **Edit** the page or snippet file in this repo (branch/PR as your team prefers).
2. **Copy or sync** the updated body into the matching **Konnect** page or snippet (Portal UI, API, or your team’s process).
3. **Set or verify** the page **slug** and **visibility** in Konnect so links and left nav match.
4. **Confirm** layout snippets, theme, and **assets** (especially `/images/...` vs external URLs) in the live portal.
5. **Commit** here so Git stays the durable record of approved copy and structure.

Header, footer, and global navigation are configured in the **Konnect theme / layout**, not in these page files.

## Page TOC (right rail)

When using `sidebar-right: "example-page-toc"` (or similar), the **Page TOC** component is driven by headings in the rendered page. In practice:

- Use **`##` for major sections** and **`###` for subsections** you want in the outline (Kong’s default depth is often H2 + H3).
- **Avoid `#` in the body** for sections you expect in the TOC—**H1** is usually not treated like other TOC entries the same way **H2/H3** are.
- If the TOC looks wrong, check whether content is split across **multiple `::page-section`** blocks; your layout/TOC snippet may only scan certain regions—**one continuous `::page-section`** for the whole article is the safest pattern when in doubt.

## Canonical examples in this repo

Use these as templates when adding new guides:

- `getting-started` — Hero + section + nested columns and snippet tiles.
- `api-key-guide` — Long-form guide with images and numbered steps.
- `bankrate-content-feeds` — Tables, technical blocks, long single section.

## Using this repo in Cursor

- Open the **folder** as a Cursor workspace so paths and search stay scoped to this project.
- This repo includes a **project Cursor rule**: [`.cursor/rules/kong-portal-mdc.mdc`](.cursor/rules/kong-portal-mdc.mdc) (`alwaysApply: true`) so agents follow Kong MDC and TOC conventions. Adjust or split that file if your team needs different scope. See [Cursor Rules](https://docs.cursor.com/context/rules-for-ai). Optional: add `AGENTS.md` for extra human-facing agent notes.
- New chats do **not** automatically read every file; a **README** plus **rules** gives collaborators and agents a consistent starting point.

## Contributing

Keep edits **scoped to the page or snippet** you are updating. When you introduce a new snippet or slug, document it in the PR or commit message so whoever syncs to Konnect knows what to create or update on the other side.
