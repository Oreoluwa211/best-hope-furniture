# BEST HOPE Furniture

A modern, single-page e-commerce storefront for BEST HOPE Furniture — built as a fast, animated shopping experience for browsing and ordering furniture online, with checkout handled via WhatsApp.

**Live site:** [best-hope-furniture.vercel.app](https://best-hope-furniture.vercel.app)

## Features

- **Product catalog** with category filters, search overlay, and quick-view modal
- **Cart & wishlist** with a slide-out drawer for each
- **WhatsApp checkout** — orders are formatted into a WhatsApp message and sent directly to the store's number, no payment gateway required
- **Animated UI** throughout (hero slider, page transitions, hover states) powered by Framer Motion
- **Showroom, testimonials, stats, and "Why Us" sections** to build trust and showcase the brand
- **Toast notifications** for cart/wishlist actions
- **Fully responsive**, mobile-first layout

## Tech Stack

- [React](https://react.dev/)
- [Vite](https://vitejs.dev/) — build tool & dev server
- [Tailwind CSS](https://tailwindcss.com/) — styling
- [Framer Motion](https://www.framer.com/motion/) — animation
- Deployed on [Vercel](https://vercel.com/)

## Getting Started

### Prerequisites

- Node.js (v18 or later recommended)
- npm

### Installation

```bash
git clone https://github.com/<Oreoluwa211>/best-hope-furniture.git
cd best-hope-furniture
npm install
```

### Development

```bash
npm run dev
```

Runs the app locally with hot reload, typically at `http://localhost:5173`.

### Build

```bash
npm run build
```

Outputs a production-ready build to the `dist/` folder.

### Preview production build

```bash
npm run preview
```

## Project Structure

```
├── src/
│   ├── App.jsx        # Main app — all sections, components, and product data
│   └── main.jsx        # React entry point
├── index.html
├── package.json
└── vite.config.js
```

> **Note:** Product images are currently embedded directly in `App.jsx` as base64 data URIs. This keeps the app self-contained with no external image hosting, at the cost of a larger source file. Consider moving to `/public` assets or an image CDN if the catalog grows significantly.

## Configuration

A few values are set directly in `App.jsx` and should be updated for your deployment:

- `WHATSAPP_NUMBER` — the store's WhatsApp number that receives checkout orders
- `ADMIN_EMAIL` — contact/admin email shown on the site
- `PRODUCTS` — the product catalog (name, price, category, image, etc.)

## Deployment

The site is deployed on Vercel. Pushing to the connected branch (typically `main`) triggers an automatic build and deploy. To deploy manually:

```bash
npm run build
```

then upload the `dist/` folder via the Vercel dashboard or CLI (`vercel --prod`).

## License

© BEST HOPE Furniture. All rights reserved.
