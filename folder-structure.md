---
icon: folder-tree
---

# Folder Structure

This page provides an overview of the **oasis-bo-web** project folder structure.&#x20;

It is intended to help internal developers quickly understand how the codebase is organized, where to find specific modules, and where to place new code consistently.

***

<table><thead><tr><th width="303">Path</th><th>Description</th></tr></thead><tbody><tr><td>📁 <strong>deploy/</strong></td><td>Deployment configuration</td></tr><tr><td><code>└─ nginx/</code></td><td>Nginx configuration for production and staging</td></tr><tr><td>📁 <strong>docker/</strong></td><td>Docker and container configuration</td></tr><tr><td><code>├─ Dockerfile</code></td><td>Docker image definition for the app</td></tr><tr><td><code>├─ Dockerfile.staging</code></td><td>Dockerfile for staging environment</td></tr><tr><td><code>├─ docker-compose.yml</code></td><td>Local Docker services definition</td></tr><tr><td><code>├─ docker-compose-prod.yml</code></td><td>Docker Compose config for production</td></tr><tr><td><code>└─ docker-compose-stg.yml</code></td><td>Docker Compose config for staging</td></tr><tr><td>🌐 <strong>public/</strong></td><td>Public assets served directly, without bundler processing</td></tr><tr><td><code>├─ images/</code></td><td>Static images and icons for UI</td></tr><tr><td><code>└─ obw/</code></td><td>App-related public assets and static files</td></tr><tr><td>💙 <strong>src/</strong></td><td>Main folder for all application source code</td></tr><tr><td><code>├─ 📁 app/</code></td><td>Application structure, pages, layouts, and UI components</td></tr><tr><td><code>│ ├─ 🧩 components/</code></td><td>Reusable UI components across pages</td></tr><tr><td><code>│ ├─ 🖼️ layouts/</code></td><td>Global layout wrappers — header, logo, page structure</td></tr><tr><td><code>│ └─ 📑 pages/</code></td><td>Feature pages by module: Dashboard, Customer, Sales, Purchase, Report…</td></tr><tr><td><code>├─ 🖼️ assets/</code></td><td>Static assets: images, icons, and other resources</td></tr><tr><td><code>├─ ⚙️ config/</code></td><td>App configuration and initial setup — env, global init</td></tr><tr><td><code>├─ 🔀 routes/</code></td><td>Route definitions for page navigation</td></tr><tr><td><code>├─ 🗄️ store/</code></td><td>Global state management — store, hooks, shared logic</td></tr><tr><td><code>├─ 🔧 utils/</code></td><td>Helpers &#x26; utilities — API client, token, local storage, custom hooks</td></tr><tr><td><code>├─ 🎨 index.css</code></td><td>Global application styles</td></tr><tr><td><code>└─ ⚡ main.jsx</code></td><td>Entry point — initializes the React/Vite app</td></tr><tr><td>📄 <strong>Root</strong></td><td>Config files at the root level</td></tr><tr><td><code>├─ ⚡ index.html</code></td><td>Main HTML entry point</td></tr><tr><td><code>├─ 📦 package.json</code></td><td>Dependencies, scripts, and project metadata</td></tr><tr><td><code>├─ 🔒 pnpm-lock.yaml</code></td><td>Package lockfile for consistent dependency versions</td></tr><tr><td><code>├─ ⚙️ postcss.config.js</code></td><td>PostCSS configuration</td></tr><tr><td><code>├─ 📖 README.md</code></td><td>General documentation and usage guide</td></tr><tr><td><code>├─ 🎨 tailwind.config.js</code></td><td>Tailwind CSS configuration</td></tr><tr><td><code>└─ ⚡ vite.config.js</code></td><td>Vite bundler configuration</td></tr></tbody></table>

***

> **Notes:**
>
> * `src/app/pages/` — main folder for feature pages.
> * `src/app/components/` — reusable components, not tied directly to a single page.
> * `src/store/` — global state shared across the entire application.
> * `src/utils/` — general helpers to keep the main codebase clean and organized.
