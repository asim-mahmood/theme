# Shopify Theme (OS 3.0) + TailwindCSS

A minimal starter Shopify theme scaffolded for Online Store 3.0 using Tailwind CSS for utility-first styling and a quick local dev workflow.

Features
- Online Store 3.0 (sections & JSON templates)
- Tailwind CSS (JIT-ready)
- Simple npm scripts for watch/build
- Works with Shopify CLI for live dev

Quick start
1. Clone
   git clone https://github.com/asim-mahmood/theme.git
   cd theme

2. Install
   npm install

3. Dev workflow (two terminals)
   - Build/watch CSS:
     npm run watch:css
   - Run Shopify dev server:
     shopify theme dev --store=your-dev-store.myshopify.com

Tailwind (example)
- src/styles/tailwind.css:
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
- tailwind.config.js content should include Liquid and JSON:
  content: [".//*.{liquid,json,js}"]

Build & deploy
- Build production CSS:
  npm run build:css
- Push to store:
  shopify theme push --store=your-store.myshopify.com

Notes & tips
- Add Tailwind safelist for classes generated in Liquid.
- Keep assets/ for compiled CSS/JS used by Shopify.
- Run accessibility and performance audits before production.

License
Choose and add a LICENSE (e.g., MIT).