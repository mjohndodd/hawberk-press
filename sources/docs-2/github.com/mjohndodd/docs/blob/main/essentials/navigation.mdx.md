# Source: https://github.com/mjohndodd/docs/blob/main/essentials/navigation.mdx

[mjohndodd](https://github.com/mjohndodd) / **[docs](https://github.com/mjohndodd/docs)** Public

- [Notifications](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs) You must be signed in to change notification settings
- [Fork 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)
- [Star 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)

 ## FilesExpand file tree

main

/

# navigation.mdx

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

[History](https://github.com/mjohndodd/docs/commits/main/essentials/navigation.mdx)

Open commit details

History

87 lines (70 loc) · 1.93 KB

main

/

# navigation.mdx

Copy path

Top

## File metadata and controls

- Preview

- Code

- Blame

87 lines (70 loc) · 1.93 KB

[Raw](https://github.com/mjohndodd/docs/raw/refs/heads/main/essentials/navigation.mdx)

Copy raw file

Download raw file

Outline

Edit and raw actions

title | Navigation
description | The navigation field in docs.json defines the pages that go in the navigation menu
icon | map

The navigation menu is the list of links on every website.

You will likely update `docs.json` every time you add a new page. Pages do not show up automatically.

## Navigation syntax

Our navigation syntax is recursive which means you can make nested navigation groups. You don't need to include `.mdx` in page names.

```json
"navigation": {
  "tabs": [
    {
      "tab": "Docs",
      "groups": [
        {
          "group": "Getting Started",
          "pages": ["quickstart"]
        }
      ]
    }
  ]
}
```

```json
"navigation": {
  "tabs": [
    {
      "tab": "Docs",
      "groups": [
        {
          "group": "Getting Started",
          "pages": [
            "quickstart",
            {
              "group": "Nested Reference Pages",
              "pages": ["nested-reference-page"]
            }
          ]
        }
      ]
    }
  ]
}
```

## Folders

Simply put your MDX files in folders and update the paths in `docs.json`.

For example, to have a page at `https://yoursite.com/your-folder/your-page` you would make a folder called `your-folder` containing an MDX file called `your-page.mdx`.

You cannot use `api` for the name of a folder unless you nest it inside another folder. Mintlify uses Next.js which reserves the top-level `api` folder for internal server calls. A folder name such as `api-reference` would be accepted.

```json
"navigation": {
  "tabs": [
    {
      "tab": "Docs",
      "groups": [
        {
          "group": "Group Name",
          "pages": ["your-folder/your-page"]
        }
      ]
    }
  ]
}
```

## Hidden pages

MDX files not included in `docs.json` will not show up in the sidebar but are accessible through the search bar and by linking directly to them.