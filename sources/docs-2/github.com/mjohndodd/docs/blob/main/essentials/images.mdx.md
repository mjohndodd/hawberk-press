# Source: https://github.com/mjohndodd/docs/blob/main/essentials/images.mdx

[mjohndodd](https://github.com/mjohndodd) / **[docs](https://github.com/mjohndodd/docs)** Public

- [Notifications](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs) You must be signed in to change notification settings
- [Fork 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)
- [Star 0](https://github.com/login?return_to=%2Fmjohndodd%2Fdocs)

 ## FilesExpand file tree

main

/

# images.mdx

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

[History](https://github.com/mjohndodd/docs/commits/main/essentials/images.mdx)

Open commit details

History

59 lines (41 loc) · 1.52 KB

main

/

# images.mdx

Copy path

Top

## File metadata and controls

- Preview

- Code

- Blame

59 lines (41 loc) · 1.52 KB

[Raw](https://github.com/mjohndodd/docs/raw/refs/heads/main/essentials/images.mdx)

Copy raw file

Download raw file

Outline

Edit and raw actions

title | Images and embeds
description | Add image, video, and other HTML elements
icon | image

<img style={{ borderRadius: '0.5rem' }} src="[https://mintlify-assets.b-cdn.net/bigbend.jpg](https://mintlify-assets.b-cdn.net/bigbend.jpg)" />

## Image

### Using Markdown

The [markdown syntax](https://www.markdownguide.org/basic-syntax/#images) lets you add images using the following code

```md
![title](/path/image.jpg)
```

Note that the image file size must be less than 5MB. Otherwise, we recommend hosting on a service like [Cloudinary](https://cloudinary.com/) or [S3](https://aws.amazon.com/s3/). You can then use that URL and embed.

### Using embeds

To get more customizability with images, you can also use [embeds](https://github.com/mjohndodd/docs/blob/main/writing-content/embed) to add images

```html
<img height="200" src="/path/image.jpg" />
```

## Embeds and HTML elements

<iframe width="560" height="315" src="[https://www.youtube.com/embed/4KzFe50RQkQ](https://www.youtube.com/embed/4KzFe50RQkQ)" title="YouTube video player" frameBorder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowFullScreen style={{ width: '100%', borderRadius: '0.5rem' }} ></iframe> 

Mintlify supports [HTML tags in Markdown](https://www.markdownguide.org/basic-syntax/#html). This is helpful if you prefer HTML tags to Markdown syntax, and lets you create documentation with infinite flexibility.

### iFrames

Loads another HTML page within the document. Most commonly used for embedding videos.

```html
<iframe src="https://www.youtube.com/embed/4KzFe50RQkQ"> </iframe>
```