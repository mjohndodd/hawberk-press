# Source: https://github.com/mjohndodd/docs/blob/main/essentials/markdown.mdx

[mjohndodd](https://github.com/mjohndodd) / **[docs](https://github.com/mjohndodd/docs)** Public

- [Notifications](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs) You must be signed in to change notification settings
- [Fork 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)
- [Star 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)

 ## FilesExpand file tree

main

/

# markdown.mdx

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

[History](https://github.com/mjohndodd/docs/commits/main/essentials/markdown.mdx)

Open commit details

History

88 lines (57 loc) · 2.51 KB

main

/

# markdown.mdx

Copy path

Top

## File metadata and controls

- Preview

- Code

- Blame

88 lines (57 loc) · 2.51 KB

[Raw](https://github.com/mjohndodd/docs/raw/refs/heads/main/essentials/markdown.mdx)

Copy raw file

Download raw file

Outline

Edit and raw actions

title | Markdown syntax
description | Text, title, and styling in standard markdown
icon | text-size

## Titles

Best used for section headers.

```md
## Titles
```

### Subtitles

Best used for subsection headers.

```md
### Subtitles
```

Each **title** and **subtitle** creates an anchor and also shows up on the table of contents on the right.

## Text formatting

We support most markdown formatting. Simply add `**`, `_`, or `~` around text to format it.

| Style | How to write it | Result |
| --- | --- | --- |
| Bold | `**bold**` | **bold** |
| Italic | `_italic_` | _italic_ |
| Strikethrough | `~strikethrough~` | ~strikethrough~ |

You can combine these. For example, write `**_bold and italic_**` to get **_bold and italic_** text.

You need to use HTML to write superscript and subscript text. That is, add `<sup>` or `<sub>` around your text.

| Text Size | How to write it | Result |
| --- | --- | --- |
| Superscript | `<sup>superscript</sup>` | superscript |
| Subscript | `<sub>subscript</sub>` | subscript |

## Linking to pages

You can add a link by wrapping text in `[]()`. You would write `[link to google](https://google.com)` to [link to google](https://google.com).

Links to pages in your docs need to be root-relative. Basically, you should include the entire folder path. For example, `[link to text](/writing-content/text)` links to the page "Text" in our components section.

Relative links like `[link to text](../text)` will open slower because we cannot optimize them as easily.

## Blockquotes

### Singleline

To create a blockquote, add a `>` in front of a paragraph.

> Dorothy followed her through many of the beautiful rooms in her castle.

```md
> Dorothy followed her through many of the beautiful rooms in her castle.
```

### Multiline

> Dorothy followed her through many of the beautiful rooms in her castle.
> 
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

```md
> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
```

### LaTeX

Mintlify supports [LaTeX](https://www.latex-project.org) through the Latex component.

8 x (vk x H1 - H2) = (0,1)

```md
<Latex>8 x (vk x H1 - H2) = (0,1)</Latex>
```