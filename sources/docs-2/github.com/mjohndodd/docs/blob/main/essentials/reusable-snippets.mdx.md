# Source: https://github.com/mjohndodd/docs/blob/main/essentials/reusable-snippets.mdx

[mjohndodd](https://github.com/mjohndodd) / **[docs](https://github.com/mjohndodd/docs)** Public

- [Notifications](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs) You must be signed in to change notification settings
- [Fork 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)
- [Star 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)

 ## FilesExpand file tree

main

/

# reusable-snippets.mdx

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

[History](https://github.com/mjohndodd/docs/commits/main/essentials/reusable-snippets.mdx)

Open commit details

History

110 lines (78 loc) · 2.52 KB

main

/

# reusable-snippets.mdx

Copy path

Top

## File metadata and controls

- Preview

- Code

- Blame

110 lines (78 loc) · 2.52 KB

[Raw](https://github.com/mjohndodd/docs/raw/refs/heads/main/essentials/reusable-snippets.mdx)

Copy raw file

Download raw file

Outline

Edit and raw actions

title | Reusable snippets
description | Reusable, custom snippets to keep content in sync
icon | recycle

import SnippetIntro from '/snippets/snippet-intro.mdx';

## Creating a custom snippet

**Pre-condition**: You must create your snippet file in the `snippets` directory.

Any page in the \`snippets\` directory will be treated as a snippet and will not be rendered into a standalone page. If you want to create a standalone page from the snippet, import the snippet into another file and call it as a component.

### Default export

1. Add content to your snippet file that you want to re-use across multiple locations. Optionally, you can add variables that can be filled in via props when you import the snippet.

```mdx
Hello world! This is my content I want to reuse across pages. My keyword of the
day is {word}.
```

The content that you want to reuse must be inside the \`snippets\` directory in order for the import to work.

2. Import the snippet into your destination file.

```mdx
---
title: My title
description: My Description
---

import MySnippet from '/snippets/path/to/my-snippet.mdx';

## Header

Lorem impsum dolor sit amet.

<MySnippet word="bananas" />
```

### Reusable variables

1. Export a variable from your snippet file:

```mdx
export const myName = 'my name';

export const myObject = { fruit: 'strawberries' };
```

2. Import the snippet from your destination file and use the variable:

```mdx
---
title: My title
description: My Description
---

import { myName, myObject } from '/snippets/path/to/custom-variables.mdx';

Hello, my name is {myName} and I like {myObject.fruit}.
```

### Reusable components

1. Inside your snippet file, create a component that takes in props by exporting your component in the form of an arrow function.

```mdx
export const MyComponent = ({ title }) => (
  <div>
    <h1>{title}</h1>
    <p>... snippet content ...</p>
  </div>
);
```

MDX does not compile inside the body of an arrow function. Stick to HTML syntax when you can or use a default export if you need to use MDX.

2. Import the snippet into your destination file and pass in the props

```mdx
---
title: My title
description: My Description
---

import { MyComponent } from '/snippets/custom-component.mdx';

Lorem ipsum dolor sit amet.

<MyComponent title={'Custom title'} />
```