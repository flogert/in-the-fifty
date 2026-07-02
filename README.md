# In The Fifty

> 🇺🇸 A website for a business that sells 100% American-made products through social media (TikTok, etc.)

## Tech Stack

- [Astro](https://astro.build/) v4 — static site framework (powered by Vite)
- Vanilla CSS with CSS custom properties
- TypeScript (strict mode)

## Project Structure

```
src/
├── components/
│   ├── Header.astro        — Sticky nav with mobile hamburger menu
│   ├── Hero.astro          — Full-height landing hero with CTAs
│   ├── FeaturedProducts.astro — Product grid showcase
│   ├── About.astro         — Our story + stats section
│   ├── ShopContact.astro   — TikTok shop links + contact form
│   └── Footer.astro        — Footer with nav & social links
├── layouts/
│   └── Layout.astro        — Base HTML layout with global CSS
└── pages/
    └── index.astro         — Main landing page
public/
└── favicon.svg
```

## Getting Started

```bash
# Install dependencies
npm install

# Start dev server (http://localhost:4321)
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Customisation Notes

- **Product images** — Replace the placeholder blocks in `FeaturedProducts.astro` with real `<img>` tags once assets are ready.
- **TikTok handle** — Update the `@inthefifty` links in `Hero.astro`, `ShopContact.astro`, and `Footer.astro` to match the live account URL.
- **Contact form** — The form in `ShopContact.astro` currently has no backend. Hook it up to a service like Formspree, Netlify Forms, or a custom API endpoint.
- **Brand colours** — Defined as CSS variables in `layouts/Layout.astro` (`--color-red`, `--color-blue`, `--color-dark`).
