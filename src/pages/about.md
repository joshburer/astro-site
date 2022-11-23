---
layout: ../layouts/BaseLayout.astro
title: About
---

# About

This site was built using <span class="astro-link">[Astro](https://astro.build/)</span> in an effort to accomplish a few things:

- Keep the JavaScript payload small and keep things minimal.
- Have the ability to edit site content with Markdown.
- Learn a new framework :)

It is hosted using Github Pages following [this guide](https://docs.astro.build/en/guides/deploy/github/).

---

## Thoughts on Astro

- SSR and zero-JS is pretty cool.
- React-style keeping HTML and JS together is intuitive and good.
  - Astro's `.astro` format does not do this well ^
    - You have to explicitly consume `class` as a prop. I appreciate not having a `className`, but it doesn't work.
    - You cannot add styles to child elements without becoming global (scope is not applied to children). There is no way to select a custom component.
    - Rules are inconsistent for returning HTML from a function. It works when mapping within `{}` in the HTML section of a file, but in the JavaScript "frontmatter" section of a `.astro` file, it does not work.
  - Upside is, you can just use whatever framework you want. [This page is in React](/react)