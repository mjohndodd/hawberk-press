# Source: https://github.com/mjohndodd/docs/blob/main/ai-tools/windsurf.mdx

[mjohndodd](https://github.com/mjohndodd) / **[docs](https://github.com/mjohndodd/docs)** Public

- [Notifications](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs) You must be signed in to change notification settings
- [Fork 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)
- [Star 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)

 ## FilesExpand file tree

main

/

# windsurf.mdx

Copy path

Blame

More file actions

Blame

More file actions

## Latest commit

[![mjohndodd](https://avatars.githubusercontent.com/u/100431911?v=4&size=40)](https://github.com/mjohndodd) [mjohndodd](https://github.com/mjohndodd/docs/commits?author=mjohndodd)

[Initial commit](https://github.com/mjohndodd/docs/commit/9efac4d5e5d99a56ad196cc977751ef27a9295af)

Oct 14, 2025

[9efac4d](https://github.com/mjohndodd/docs/commit/9efac4d5e5d99a56ad196cc977751ef27a9295af) · Oct 14, 2025

## History

[History](https://github.com/mjohndodd/docs/commits/main/ai-tools/windsurf.mdx)

Open commit details

History

96 lines (69 loc) · 2.69 KB

main

/

# windsurf.mdx

Copy path

Top

## File metadata and controls

- Preview

- Code

- Blame

96 lines (69 loc) · 2.69 KB

[Raw](https://github.com/mjohndodd/docs/raw/refs/heads/main/ai-tools/windsurf.mdx)

Copy raw file

Download raw file

Outline

Edit and raw actions

title | Windsurf setup
description | Configure Windsurf for your documentation workflow
icon | water

Configure Windsurf's Cascade AI assistant to help you write and maintain documentation. This guide shows how to set up Windsurf specifically for your Mintlify documentation workflow.

## Prerequisites

- Windsurf editor installed
- Access to your documentation repository

## Workspace rules

Create workspace rules that provide Windsurf with context about your documentation project and standards.

Create `.windsurf/rules.md` in your project root:

```md
# Mintlify technical writing rule

## Project context

- This is a documentation project on the Mintlify platform
- We use MDX files with YAML frontmatter  
- Navigation is configured in `docs.json`
- We follow technical writing best practices

## Writing standards

- Use second person ("you") for instructions
- Write in active voice and present tense
- Start procedures with prerequisites
- Include expected outcomes for major steps
- Use descriptive, keyword-rich headings
- Keep sentences concise but informative

## Required page structure

Every page must start with frontmatter:

```yaml
---
title: "Clear, specific title"
description: "Concise description for SEO and navigation"
---
```

## Mintlify components

### Callouts

- `<Note>` for helpful supplementary information
- `<Warning>` for important cautions and breaking changes
- `<Tip>` for best practices and expert advice 
- `<Info>` for neutral contextual information
- `<Check>` for success confirmations

### Code examples

- When appropriate, include complete, runnable examples
- Use `<CodeGroup>` for multiple language examples
- Specify language tags on all code blocks
- Include realistic data, not placeholders
- Use `<RequestExample>` and `<ResponseExample>` for API docs

### Procedures

- Use `<Steps>` component for sequential instructions
- Include verification steps with `<Check>` components when relevant
- Break complex procedures into smaller steps

### Content organization

- Use `<Tabs>` for platform-specific content
- Use `<Accordion>` for progressive disclosure
- Use `<Card>` and `<CardGroup>` for highlighting content
- Wrap images in `<Frame>` components with descriptive alt text

## API documentation requirements

- Document all parameters with `<ParamField>` 
- Show response structure with `<ResponseField>`
- Include both success and error examples
- Use `<Expandable>` for nested object properties
- Always include authentication examples

## Quality standards

- Test all code examples before publishing
- Use relative paths for internal links
- Include alt text for all images
- Ensure proper heading hierarchy (start with h2)
- Check existing patterns for consistency
```