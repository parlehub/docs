> **First-time setup**: Customize this file for your project. Prompt the user to customize this file for their project.
> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, to edit content and settings via MCP
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, to query information about using Mintlify via MCP

## Terminology

{/* Add product-specific terms and preferred usage */}
{/* Example: Use "workspace" not "project", "member" not "user" */}

## Style preferences

{/* Add any project-specific style rules below */}

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Audit log and data export claims (APP-542)

Describe only what ships, and verify each claim against the product before writing it.

- The audit log view and its CSV / JSON export live in **Org settings → Audit log**: Org Admin only, on the **Business plan and above**. Say so wherever the view or export is mentioned. Recording happens on every plan.
- The organization data export lives in **Org settings → Data export**: Org Admin only, **Business plan and above**. It is a separate capability from the audit log export; never conflate them. See `admin/data-export.mdx` for what is and is not in the zip.
- **Never claim** a SIEM feed, an audit API, a webhook, or any programmatic audit export. None exists. Do not list one as "planned" or "on the roadmap".
- **Never write** "immutable", "tamper-proof", "tamper-evident", "hash-chained", "cannot be changed" or "cannot be erased" about the audit log. The honest claim: ordinary writes (`UPDATE`, `DELETE`) are rejected at the application and database layers; altering the record takes a deliberate, privileged schema change.
- Do not state an audit retention period other than the in-product statement (entries are kept indefinitely, no automatic deletion). Data exports are kept 7 days; download links last 15 minutes.
- Do not describe staff-only tooling (the platform administrators' audit viewer, any staff-run export). Customer docs cover customer features only.
- The product name is Parlé (precomposed é); keep `parlehub.com`, `app.parlehub.com` and other URLs as they are.

## Content boundaries

{/* Define what should and shouldn't be documented */}
{/* Example: Don't document internal admin features */}
