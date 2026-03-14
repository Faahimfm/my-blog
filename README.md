# Faahim Blog — Astro Project

## Getting Started

```bash
npm install
npm run dev      # start dev server at localhost:4321
npm run build    # build for production
npm run preview  # preview production build
```

---

## How to Write a New Article

1. Create a new file in `src/content/articles/`
2. Name it anything — e.g. `my-new-post.md`
3. Add frontmatter at the top, then write in Markdown

**Template:**

```md
---
title: "Your Article Title"
description: "One sentence summary shown on the articles listing page."
date: "2024-03-15"
slug: "your-article-url-slug"
---

Write your article here in Markdown.

## A Heading

Normal paragraph text. Add as many sections as you like.

## Code Example

    ```js
    const hello = "world";
    ```
```

That's it. The article will appear automatically on `/articles` sorted by date, and will be readable at `/articles/your-article-url-slug`.

---

## Updating Your Info

| What                  | File                              |
|-----------------------|-----------------------------------|
| Name, subtitle, links | `src/pages/index.astro`           |
| Portfolio URL         | `src/pages/index.astro` (hero btn)|
| Timeline entries      | `src/pages/journey.astro`         |
| Social links          | `src/pages/contact.astro`         |
| Email address         | `src/pages/contact.astro`         |
| Global styles/colors  | `src/styles/global.css`           |

---

## Project Structure

```
faahim-blog/
├── src/
│   ├── content/
│   │   └── articles/        ← your .md articles go here
│   ├── layouts/
│   │   └── BaseLayout.astro ← nav, footer, <head> shared across all pages
│   ├── pages/
│   │   ├── index.astro      ← home (hero)
│   │   ├── journey.astro    ← timeline
│   │   ├── contact.astro    ← contact + social links
│   │   └── articles/
│   │       ├── index.astro  ← article listing (auto-generated)
│   │       └── [slug].astro ← individual article pages (auto-generated)
│   └── styles/
│       └── global.css       ← all CSS
└── public/
    └── favicon.svg
```
