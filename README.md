# Astro Components

Astro 0.25 &npx astro add Tailwind CSS 1.0.23

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

## Project Structure

```
/
├── public/
├── src/
│   └── pages/
│       └── index.astro
└── package.json
```
