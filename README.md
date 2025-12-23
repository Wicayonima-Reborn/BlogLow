# Blog

Personal programming notes and articles built with **Astro** and deployed to **GitHub Pages**.

This repository contains a simple, fast, and static blog setup using Astro Content Collections. The focus is on writing and sharing programming-related articles without complex tooling.

---

## 🚀 Tech Stack

* **Astro** — static site generator
* **Markdown / MDX** — content authoring
* **Astro Content Collections** — typed content management
* **GitHub Pages** — free static hosting

---

## 📂 Project Structure

```
src/
├─ pages/
│  ├─ index.astro          # Home page
│  ├─ blog/
│  │  ├─ index.astro       # Blog list
│  │  └─ [slug].astro      # Blog post page
│  └─ about.astro
│
├─ content/
│  └─ blog/                # Blog posts (Markdown / MDX)
│
├─ components/             # Reusable UI components
├─ layouts/                # Page layouts
└─ content/config.ts       # Content schema
```

---

## ✍️ Writing a Blog Post

Create a new Markdown file inside:

```
src/content/blog/
```

Example:

```md
---
title: "What is Low-Level Programming?"
description: "A short introduction to low-level concepts"
pubDate: 2025-01-01
tags: ["systems", "programming"]
draft: false
---

Your content starts here.
```

### Draft Posts

To hide a post from the site, set:

```yaml
draft: true
```

Draft posts will not appear on the home page or blog list.

---

## 🧪 Development

Install dependencies:

```bash
npm install
```

Run the local dev server:

```bash
npm run dev
```

The site will be available at:

```
http://localhost:4321
```

---

## 📦 Build

Generate a production build:

```bash
npm run build
```

Preview the build locally:

```bash
npm run preview
```

---

## 🌍 Deployment

The site is deployed automatically using **GitHub Actions** to **GitHub Pages**.

Production URL:

```
https://wicayonima-reborn.github.io/Blog/
```

Astro is configured to handle the GitHub Pages base path correctly.

---

## 🤝 Contributing

Contributions are welcome.

Basic flow:

1. Fork this repository
2. Create a new Markdown file in `src/content/blog/`
3. Commit and open a Pull Request

Please keep articles focused on programming or software development topics.

---

## 📄 License

This project is open for educational and personal use.