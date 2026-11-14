# Paradise Nursery Shopping Cart Application (e-plantShopping)

A shopping cart application for an online plant shop, built with React and Redux Toolkit as the final project of the IBM **Developing Front-End Apps with React** course (Coursera).

**Live app (GitHub Pages):** https://marysegahou.github.io/e-plantShopping/

**Author:** Maryse GAHOU

## Features

- **Landing page** — background image, company name ("Welcome To Paradise Nursery — Where Green Meets Serenity"), an About Us paragraph and a **Get Started** button linking to the product listing page.
- **Product listing page** — 5 categories of plants (Air Purifying, Aromatic Fragrant, Insect Repellent, Medicinal, Low Maintenance), 6 plants per category. Each plant card shows a thumbnail, name, description, cost and an **Add to Cart** button (the button is disabled once the plant has been added). The navbar shows the live quantity of items in the cart next to the cart icon.
- **Shopping cart page** — a card per plant type in the cart with thumbnail, name, unit cost, quantity stepper (+/−), total cost per plant and a **Delete** button. Displays the total cart amount, **Continue Shopping** (returns to the listing) and **Checkout** (shows "Coming Soon").
- **Navigation bar** with links to the landing page (logo), the plant listing (**Plants**) and the shopping cart (cart icon).

## Technologies

- React 18 (functional components, hooks: `useState`, `useEffect`)
- Redux Toolkit (`createSlice`, `configureStore`) with `react-redux`
- Vite

## Project structure

- `src/App.jsx` — landing page and navigation to the product listing
- `src/AboutUs.jsx` — company description shown on the landing page
- `src/ProductList.jsx` — plant catalogue, navbar and "Add to Cart" logic
- `src/CartItem.jsx` — cart page (totals, quantity steppers, delete)
- `src/CartSlice.jsx` — Redux slice (`addItem`, `removeItem`, `updateQuantity`)
- `src/store.js` — Redux store

## Getting started

```bash
npm install
npm run dev
```

## Build & deploy (GitHub Pages)

```bash
npm run build
npm run deploy   # publishes the dist folder to the gh-pages branch
```
