# Source: https://github.com/mjohndodd/docs/blob/main/api-reference/introduction.mdx

[mjohndodd](https://github.com/mjohndodd) / **[docs](https://github.com/mjohndodd/docs)** Public

- [Notifications](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs) You must be signed in to change notification settings
- [Fork 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)
- [Star 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)

 ## FilesExpand file tree

main

/

# introduction.mdx

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

[History](https://github.com/mjohndodd/docs/commits/main/api-reference/introduction.mdx)

Open commit details

History

33 lines (26 loc) · 875 Bytes

main

/

# introduction.mdx

Copy path

Top

## File metadata and controls

- Preview

- Code

- Blame

33 lines (26 loc) · 875 Bytes

[Raw](https://github.com/mjohndodd/docs/raw/refs/heads/main/api-reference/introduction.mdx)

Copy raw file

Download raw file

Outline

Edit and raw actions

title | Introduction
description | Example section for showcasing API endpoints

If you're not looking to build API reference documentation, you can delete this section by removing the api-reference folder.

## Welcome

There are two ways to build API documentation: [OpenAPI](https://mintlify.com/docs/api-playground/openapi/setup) and [MDX components](https://mintlify.com/docs/api-playground/mdx/configuration). For the starter kit, we are using the following OpenAPI specification.

<Card title="Plant Store Endpoints" icon="leaf" href="[https://github.com/mintlify/starter/blob/main/api-reference/openapi.json](https://github.com/mintlify/starter/blob/main/api-reference/openapi.json)"

View the OpenAPI specification file

## Authentication

All API endpoints are authenticated using Bearer tokens and picked up from the specification file.

```json
"security": [
  {
    "bearerAuth": []
  }
]
```