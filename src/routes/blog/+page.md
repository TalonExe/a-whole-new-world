---
title: "My First Blog Post"
date: "2023-10-27"
description: "This is the first post on my new blog, powered by SvelteKit and mdsvex!"
---

## Welcome to my Blog!

This is the first post. SvelteKit and mdsvex make this incredibly easy.

You can write normal Markdown, and it will be rendered as HTML.

### Code Blocks

One of the best features is syntax highlighting for code blocks, which we configured with `shiki`.

```javascript
// src/routes/blog/+page.server.js
export async function load() {
    // ... magic happens here
    return { posts };
}