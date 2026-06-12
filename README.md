# abdallahattie.com

Personal website and blog of Abdallah Attie, built with [Astro](https://astro.build).

## Commands

| Command           | Action                                       |
| ----------------- | -------------------------------------------- |
| `npm install`     | Install dependencies                         |
| `npm run dev`     | Start local dev server at `localhost:4321`   |
| `npm run build`   | Build the production site to `./dist/`       |
| `npm run preview` | Preview the production build locally         |

## Writing a post

Add a Markdown file to `src/content/blog/`:

```markdown
---
title: 'My post title'
description: 'One-sentence summary shown in lists and feeds.'
pubDate: 2026-06-12
---

Post body in Markdown...
```

Set `draft: true` in the frontmatter to keep a post out of the published site.
The filename becomes the URL: `my-post.md` → `/blog/my-post/`.

## Personal details

Name, role, bio, and social links all live in [`src/consts.ts`](src/consts.ts).
Edit that one file to update them everywhere.

## Deploying to GitHub Pages (abdallahattie.com)

1. Create a GitHub repository and push this project to the `main` branch.
2. In the repo: **Settings → Pages → Build and deployment → Source: GitHub Actions**.
   The included workflow (`.github/workflows/deploy.yml`) builds and deploys on every push.
3. In **Settings → Pages → Custom domain**, enter `abdallahattie.com`
   (the `public/CNAME` file keeps this setting across deploys).
4. At your DNS provider, add these records:

   | Type  | Host | Value             |
   | ----- | ---- | ----------------- |
   | A     | `@`  | `185.199.108.153` |
   | A     | `@`  | `185.199.109.153` |
   | A     | `@`  | `185.199.110.153` |
   | A     | `@`  | `185.199.111.153` |
   | CNAME | `www`| `<your-github-username>.github.io` |

5. Back in GitHub Pages settings, check **Enforce HTTPS** once the certificate
   is issued (can take a few minutes after DNS propagates).
