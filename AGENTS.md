# SKUtrak Knowledge Base — Documentation Style Guide

This file defines the writing and structural conventions for the SKUtrak knowledge base hosted on Mintlify. Mintlify's writing agent and any contributor should follow these rules.

## Audience

Every article serves two readers simultaneously:

- **Humans**: Busy CPG brand users (account managers, supply chain analysts, data managers) who need to understand what they're looking at and what to do
- **AI agents**: SKUtrak's Agent Studio, Mintlify's AI Assistant, and any MCP-connected tool querying the docs for answers

## Page Structure

Every page follows this template in order:

1. **Frontmatter** — `title`, `sidebarTitle`, `description`, `icon` (all required)
2. **TL;DR** — `<Tip>` component, 2-3 sentences max, front-loads the answer
3. **Video embed** — `<Frame>` with `<iframe>` (30-second Loom when available)
4. **Role-specific framing** — `<Tabs>` with three tabs: Account Managers, Supply Chain, Data Managers
5. **Core content** — structured with `<Steps>`, `<CardGroup>`, `<Warning>`, `<Note>` as appropriate
6. **Next steps** — `<CardGroup>` with `<Card href>` links to related pages

## Voice and Tone

- Write like explaining something to a smart colleague — not writing a user manual
- Use "you" and "your" throughout
- Short sentences. Short paragraphs. Maximum 3 sentences per paragraph
- Prefer concrete examples over abstract explanations
- Never use "it's crucial", "it's important", "powerful", "seamless", "cutting-edge", or "robust"
- No emojis in body text
- Show why something matters through consequences, not assertions

## Headings

- Headings are questions or actions, never labels
- Good: "What goes wrong without clean mappings?" / "How do I upload product definitions?"
- Bad: "Common Issues" / "Upload Process"

## Terminology (strict)

Use these terms consistently. Do not use alternatives:

| Correct | Do not use |
|---------|-----------|
| Product Catalogue | product catalog, mapping tool, product management |
| mapping | linking, connecting, associating |
| product definition | product master, master product, product record |
| retailer code | retailer SKU, retailer product code (acceptable but prefer "retailer code") |
| unique code | internal code, supplier code (acceptable but prefer "unique code") |

## Mintlify Components

| Element | Component | When to use |
|---------|-----------|-------------|
| TL;DR summary | `<Tip>` | Opening summary, 2-3 sentences |
| Role-specific content | `<Tabs>` with `<Tab>` | Persona-specific framing |
| Warning / consequence | `<Warning>` | "If you don't do X, Y breaks" |
| Pro tips | `<Note>` | Practical time-saving advice |
| Scenario cards | `<CardGroup>` + `<Card>` | "What goes wrong" patterns |
| Sequential steps | `<Steps>` + `<Step>` | Any how-to process |
| Video embeds | `<Frame>` + `<iframe>` | 30-second video guides |
| Navigation links | `<CardGroup>` + `<Card href>` | "Where to go next" |
| Confirmation | `<Check>` | "You've done this correctly when..." |

## AI-Readability Rules

1. **Front-load answers**: First sentence of every section should directly answer the implied question
2. **One concept per section**: Sections should be self-contained — the MCP server returns sections, not full pages
3. **Structured headings as questions**: Match how a user would ask the AI
4. **Explicit cross-references**: Use descriptive link text, never "click here"
5. **Metadata in frontmatter**: The `description` field should be a one-sentence summary an AI can use as a snippet

## File Naming

- Use kebab-case: `product-mappings.mdx`, `map-retailer-codes.mdx`
- Names should be short and descriptive — match the `sidebarTitle` where possible
- All docs files use `.mdx` extension
