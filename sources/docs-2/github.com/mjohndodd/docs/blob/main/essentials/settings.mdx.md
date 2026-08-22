# Source: https://github.com/mjohndodd/docs/blob/main/essentials/settings.mdx

[mjohndodd](https://github.com/mjohndodd) / **[docs](https://github.com/mjohndodd/docs)** Public

- [Notifications](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs) You must be signed in to change notification settings
- [Fork 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)
- [Star 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)

 ## FilesExpand file tree

main

/

# settings.mdx

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

[History](https://github.com/mjohndodd/docs/commits/main/essentials/settings.mdx)

Open commit details

History

318 lines (266 loc) · 11.1 KB

main

/

# settings.mdx

Copy path

Top

## File metadata and controls

- Preview

- Code

- Blame

318 lines (266 loc) · 11.1 KB

[Raw](https://github.com/mjohndodd/docs/raw/refs/heads/main/essentials/settings.mdx)

Copy raw file

Download raw file

Edit and raw actions

title | Global Settings
description | Mintlify gives you complete control over the look and feel of your documentation using the docs.json file
icon | gear

Every Mintlify site needs a `docs.json` file with the core configuration settings. Learn more about the [properties](https://github.com/mjohndodd/docs/blob/main/essentials/settings.mdx#properties) below.

## Properties

Name of your project. Used for the global title.

Example: `mintlify`

An array of groups with all the pages within that group The name of the group.

```
Example: `Settings`

</ResponseField>
<ResponseField name="pages" type="string[]">
The relative paths to the markdown files that will serve as pages.

Example: `["customization", "page"]`

</ResponseField>
```

Path to logo image or object with path to "light" and "dark" mode logo images Path to the logo in light mode Path to the logo in dark mode Where clicking on the logo links you to Path to the favicon image Hex color codes for your global theme The primary color. Used for most often for highlighted content, section headers, accents, in light mode The primary color for dark mode. Used for most often for highlighted content, section headers, accents, in dark mode The primary color for important buttons The color of the background in both light and dark mode The hex color code of the background in light mode The hex color code of the background in dark mode Array of \`name\`s and \`url\`s of links you want to include in the topbar The name of the button.

```
Example: `Contact us`
</ResponseField>
<ResponseField name="url" type="string">
The url once you click on the button. Example: `https://mintlify.com/docs`
</ResponseField>
```

Link shows a button. GitHub shows the repo information at the url provided including the number of GitHub stars. If \`link\`: What the button links to.

```
If `github`: Link to the repository to load GitHub information from.
</ResponseField>
<ResponseField name="name" type="string">
Text inside the button. Only required if `type` is a `link`.
</ResponseField>
```

Array of version names. Only use this if you want to show different versions of docs with a dropdown in the navigation bar. An array of the anchors, includes the \`icon\`, \`color\`, and \`url\`. The \[Font Awesome\]([https://fontawesome.com/search?q=heart](https://fontawesome.com/search?q=heart)) icon used to feature the anchor.

```
Example: `comments`
</ResponseField>
<ResponseField name="name" type="string">
The name of the anchor label.

Example: `Community`
</ResponseField>
<ResponseField name="url" type="string">
  The start of the URL that marks what pages go in the anchor. Generally, this is the name of the folder you put your pages in.
</ResponseField>
<ResponseField name="color" type="string">
  The hex color of the anchor icon background. Can also be a gradient if you pass an object with the properties `from` and `to` that are each a hex color.
</ResponseField>
<ResponseField name="version" type="string">
  Used if you want to hide an anchor until the correct docs version is selected.
</ResponseField>
<ResponseField name="isDefaultHidden" type="boolean" default="false">
  Pass `true` if you want to hide the anchor until you directly link someone to docs inside it.
</ResponseField>
<ResponseField name="iconType" default="duotone" type="string">
  One of: "brands", "duotone", "light", "sharp-solid", "solid", or "thin"
</ResponseField>
```

Override the default configurations for the top-most anchor. The name of the top-most anchor Font Awesome icon. One of: "brands", "duotone", "light", "sharp-solid", "solid", or "thin" An array of navigational tabs. The name of the tab label. The start of the URL that marks what pages go in the tab. Generally, this is the name of the folder you put your pages in. Configuration for API settings. Learn more about API pages at \[API Components\](/api-playground/demo). The base url for all API endpoints. If \`baseUrl\` is an array, it will enable for multiple base url options that the user can toggle.

```
<ResponseField name="auth" type="Auth">
  <Expandable title="Auth">
    <ResponseField name="method" type='"bearer" | "basic" | "key"'>
      The authentication strategy used for all API endpoints.
    </ResponseField>
    <ResponseField name="name" type="string">
    The name of the authentication parameter used in the API playground.

    If method is `basic`, the format should be `[usernameName]:[passwordName]`
    </ResponseField>
    <ResponseField name="inputPrefix" type="string">
    The default value that's designed to be a prefix for the authentication input field.

    E.g. If an `inputPrefix` of `AuthKey` would inherit the default input result of the authentication field as `AuthKey`.
    </ResponseField>
  </Expandable>
</ResponseField>

<ResponseField name="playground" type="Playground">
  Configurations for the API playground

  <Expandable title="Playground">
    <ResponseField name="mode" default="show" type='"show" | "simple" | "hide"'>
      Whether the playground is showing, hidden, or only displaying the endpoint with no added user interactivity `simple`

      Learn more at the [playground guides](/api-playground/demo)
    </ResponseField>
  </Expandable>
</ResponseField>

<ResponseField name="maintainOrder" type="boolean">
  Enabling this flag ensures that key ordering in OpenAPI pages matches the key ordering defined in the OpenAPI file.

  <Warning>This behavior will soon be enabled by default, at which point this field will be deprecated.</Warning>
</ResponseField>
```

A string or an array of strings of URL(s) or relative path(s) pointing to your OpenAPI file.

Examples: `json Absolute "openapi": "https://example.com/openapi.json"` `json Relative "openapi": "/openapi.json"` `json Multiple "openapi": ["https://example.com/openapi1.json", "/openapi2.json", "/openapi3.json"]`

An object of social media accounts where the key:property pair represents the social media platform and the account url.

Example:

```json
{
  "x": "https://x.com/mintlify",
  "website": "https://mintlify.com"
}
```

One of the following values \`website\`, \`facebook\`, \`x\`, \`discord\`, \`slack\`, \`github\`, \`linkedin\`, \`instagram\`, \`hacker-news\`

```
Example: `x`
</ResponseField>
<ResponseField name="property" type="string">
The URL to the social platform.

Example: `https://x.com/mintlify`
</ResponseField>
```

Configurations to enable feedback buttons Enables a button to allow users to suggest edits via pull requests Enables a button to allow users to raise an issue about the documentation Customize the dark mode toggle. Set if you always want to show light or dark mode for new users. When not set, we default to the same mode as the user's operating system. Set to true to hide the dark/light mode toggle. You can combine \`isHidden\` with \`default\` to force your docs to only use light or dark mode. For example:

````
  <CodeGroup>
  ```json Only Dark Mode
  "modeToggle": {
    "default": "dark",
    "isHidden": true
  }
  ```

  ```json Only Light Mode
  "modeToggle": {
    "default": "light",
    "isHidden": true
  }
  ```
  </CodeGroup>

</ResponseField>
````

A background image to be displayed behind every page. See example with \[Infisical\]([https://infisical.com/docs](https://infisical.com/docs)) and \[FRPC\]([https://frpc.io](https://frpc.io)).