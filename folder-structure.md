---
icon: folder-tree
---

# Folder Structure

This page provides an overview of the **oasis-bo-web** project folder structure.&#x20;

It is intended to help internal developers quickly understand how the codebase is organized, where to find specific modules, and where to place new code consistently.

***

```
📁 deploy/
└─ 📁 nginx/          Nginx configuration for production and staging

📁 docker/
├─ 📄 Dockerfile              Docker image definition for the app
├─ 📄 Dockerfile.staging      Dockerfile for staging environment
├─ 📄 docker-compose.yml      Local Docker services definition
├─ 📄 docker-compose-prod.yml Docker Compose config for production
└─ 📄 docker-compose-stg.yml  Docker Compose config for staging

📁 public/
├─ 📁 images/   Static images and icons for UI
└─ 📁 obw/      App-related public assets and static files

📁 src/
├─ 📁 app/
│  ├─ 🧩 components/  Reusable UI components across pages
│  ├─ 🖼️ layouts/     Global layout wrappers — header, logo, page structure
│  └─ 📑 pages/       Feature pages by module: Dashboard, Customer, Sales, Purchase, Report…
├─ 🖼️ assets/         Static assets: images, icons, and other resources
├─ ⚙️ config/         App configuration and initial setup — env, global init
├─ 🔀 routes/         Route definitions for page navigation
├─ 🗄️ store/          Global state management — store, hooks, shared logic
├─ 🔧 utils/          Helpers & utilities — API client, token, local storage, custom hooks
├─ 🎨 index.css       Global application styles
└─ ⚡ main.jsx        Entry point — initializes the React/Vite app

📄 index.html          Main HTML entry point
📦 package.json        Dependencies, scripts, and project metadata
🔒 pnpm-lock.yaml      Package lockfile for consistent dependency versions
⚙️ postcss.config.js   PostCSS configuration
📖 README.md           General documentation and usage guide
🎨 tailwind.config.js  Tailwind CSS configuration
⚡ vite.config.js      Vite bundler configuration
```

***

> **Notes:**
>
> * `src/app/pages/` — main folder for feature pages.
> * `src/app/components/` — reusable components, not tied directly to a single page.
> * `src/store/` — global state shared across the entire application.
> * `src/utils/` — general helpers to keep the main codebase clean and organized.
