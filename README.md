# Astro Components

Deploy on Netlify with https://astro-tailwind-components.netlify.app/

Astro 0.25 & Tailwind CSS 1.0.23

All sorts of Tailwind components from different websites

## Silverstone

* /astro/netlify/components/
* npm init astro
* Minimal
* npm install
* npx astro add tailwind

```
astro.config.mjs ─────────────────────────────╮
 │ import { defineConfig } from 'astro/config';  │
 │                                               │
 │ import tailwind from "@astrojs/tailwind";     │
 │                                               │
 │ // https://astro.build/config                 │
 │ export default defineConfig({                 │
 │   integrations: [tailwind()]                  │
 │ });
 ```
 
 * npm install --save-dev @astrojs/tailwind
 * Astro will generate a minimal ./tailwind.config.cjs file
 * create /src/style/global.css:

```
global.css ──────────────╮
 │ @tailwind base;       │
 │ @tailwind components; │
 │ @tailwind utilities;  │
 ```

 * /src/pages/index.astro:

```
index.astro ─────────────────────╮
 │ ---                           │
 │ import '../styles/global.css' │
 │ ---                           │
 ```

* npm install --save-dev @tailwindcss/typography

```
tailwind.config.cjs ────────────────────────╮
 │ plugins: [                               │
 │      require('@tailwindcss/typography'), │
 │      // ...                              │
 │    ],                                    │
 ```

## Project Structure

```
/
├── public/
├── src/
│   └── pages/
│       └── index.astro
└── package.json
```
