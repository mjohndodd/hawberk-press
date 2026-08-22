# Source: https://github.com/mjohndodd/docs/blob/main/ai-tools/claude-code.mdx

[mjohndodd](https://github.com/mjohndodd) / **[docs](https://github.com/mjohndodd/docs)** Public

- [Notifications](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs) You must be signed in to change notification settings
- [Fork 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)
- [Star 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)

 ## FilesExpand file tree

main

/

# claude-code.mdx

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

[History](https://github.com/mjohndodd/docs/commits/main/ai-tools/claude-code.mdx)

Open commit details

History

76 lines (59 loc) · 2.39 KB

main

/

# claude-code.mdx

Copy path

Top

## File metadata and controls

- Preview

- Code

- Blame

76 lines (59 loc) · 2.39 KB

[Raw](https://github.com/mjohndodd/docs/raw/refs/heads/main/ai-tools/claude-code.mdx)

Copy raw file

Download raw file

Outline

Edit and raw actions

title | Claude Code setup
description | Configure Claude Code for your documentation workflow
icon | asterisk

Claude Code is Anthropic's official CLI tool. This guide will help you set up Claude Code to help you write and maintain your documentation.

## Prerequisites

- Active Claude subscription (Pro, Max, or API access)

## Setup

1. Install Claude Code globally:

```shell
npm install -g @anthropic-ai/claude-code
```

2. Navigate to your docs directory.
3. (Optional) Add the `CLAUDE.md` file below to your project.
4. Run `claude` to start.

## Create `CLAUDE.md`

Create a `CLAUDE.md` file at the root of your documentation repository to train Claude Code on your specific documentation standards:

```md
# Mintlify documentation

## Working relationship
- You can push back on ideas-this can lead to better documentation. Cite sources and explain your reasoning when you do so
- ALWAYS ask for clarification rather than making assumptions
- NEVER lie, guess, or make up information

## Project context
- Format: MDX files with YAML frontmatter
- Config: docs.json for navigation, theme, settings
- Components: Mintlify components

## Content strategy
- Document just enough for user success - not too much, not too little
- Prioritize accuracy and usability of information
- Make content evergreen when possible
- Search for existing information before adding new content. Avoid duplication unless it is done for a strategic reason
- Check existing patterns for consistency
- Start by making the smallest reasonable changes

## Frontmatter requirements for pages
- title: Clear, descriptive page title
- description: Concise summary for SEO/navigation

## Writing standards
- Second-person voice ("you")
- Prerequisites at start of procedural content
- Test all code examples before publishing
- Match style and formatting of existing pages
- Include both basic and advanced use cases
- Language tags on all code blocks
- Alt text on all images
- Relative paths for internal links

## Git workflow
- NEVER use --no-verify when committing
- Ask how to handle uncommitted changes before starting
- Create a new branch when no clear branch exists for changes
- Commit frequently throughout development
- NEVER skip or disable pre-commit hooks

## Do not
- Skip frontmatter on any MDX file
- Use absolute URLs for internal links
- Include untested code examples
- Make assumptions - always ask for clarification
```