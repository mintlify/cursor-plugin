# Mintlify Cursor plugin

A Cursor plugin that gives Cursor a comprehensive reference for building [Mintlify](https://mintlify.com) sites.

## What it does

Installs a `mintlify` skill and writing rules that Cursor can use when working on Mintlify-powered sites.

The skill covers:

- **Components** — Full syntax and props for all Mintlify components (callouts, cards, steps, tabs, accordions, code groups, fields, frames, and more)
- **Configuration** — Complete `docs.json` settings reference including theme, colors, logo, fonts, navbar, footer, redirects, integrations, and custom CSS/JS
- **Navigation** — All navigation patterns: groups, tabs, anchors, dropdowns, products, versions, and languages
- **API docs** — OpenAPI and AsyncAPI setup, endpoint pages, API playground configuration
- **CLI** — Full reference for every `mint` CLI command and flag

## Installation

Install from the [Cursor Marketplace](https://cursor.com/marketplace). Plugins can be installed at the user level or scoped to a project.

## MCP setup

This plugin includes two Mintlify MCP servers that are activated automatically when you install the plugin.

- **Mintlify** — Read-only access to Mintlify's published documentation. Use to look up component signatures, config options, and guides.
- **Mintlify MCP** — Write access to your Mintlify project. Requires OAuth on first use. Enables editing content, restructuring navigation, and opening pull requests directly from Cursor.

## Skills included

### `mintlify`

The skill loads a concise core reference and routes to detailed reference files only when the task requires them:

| Reference file | Contents |
|----------------|----------|
| `reference/components.md` | All component syntax, props, and examples |
| `reference/configuration.md` | Full `docs.json` schema and frontmatter fields |
| `reference/navigation.md` | Navigation patterns and when to use each |
| `reference/api-docs.md` | API documentation setup and playground config |
| `reference/cli.md` | CLI commands and flags |

## Rules included

### `rules/mintlify.mdc`

Always-on writing guardrails that activate when editing `.mdx` files or `docs.json`. Covers:

- File conventions and naming
- Internal link format (root-relative, no extensions)
- Required page frontmatter
- Writing standards (voice, headings, code blocks, alt text)
- Common mistakes to avoid

## License

MIT
