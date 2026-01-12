# Better Tech Now — Frontend (Vanilla JS)

E-commerce front-end built with vanilla JavaScript featuring product listing, filtering, search, cart system, and ratings.

## Table of contents

- [About](#about)
- [Features](#features)
- [Demo](#demo)
- [Getting started](#getting-started)
- [Usage](#usage)
- [Project structure](#project-structure)
- [Customizing products & data](#customizing-products--data)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## About

This repository contains a small, dependency-free front-end for an e-commerce experience built using plain (vanilla) JavaScript, HTML and CSS. It demonstrates product listing, client-side filtering and searching, a cart with persistence (localStorage), and a simple product rating UI.

It's ideal for learning DOM manipulation, application state without frameworks, and small static site deployments.

## Features

- Product listing (grid/list view)
- Search by product title/description
- Filter by category, price range, rating (configurable)
- Sort (e.g., price low→high, rating)
- Add/remove items from cart, update quantities
- Cart persistence using localStorage
- Simple rating display and rating input
- Responsive layout suitable for desktop/tablet/mobile
- No build step or bundler required

## Demo

To preview the app locally, open `index.html` in your browser or serve the folder with a static server (recommended).

## Getting started

Prerequisites
- Modern browser (Chrome, Firefox, Edge, Safari)
- Optional: a static server (Live Server extension, `http-server`, Python simple server)

Clone the repository:
```bash
git clone https://github.com/thatoneluckyguy/Better-Tech-Now-JS-.git
cd Better-Tech-Now-JS-
```

Open locally:
- Quick (no server): open `index.html` directly in your browser.
- Recommended (avoids file:// issues): run a local static server:

Using Node http-server:
```bash
npx http-server -c-1 .
# then open http://localhost:8080 (port may vary)
```

Using Python 3:
```bash
python -m http.server 8000
# open http://localhost:8000
```

Using VS Code Live Server: right-click `index.html` → "Open with Live Server".

## Usage

- Browse the product list or use the search field to quickly find items.
- Apply filters (category / price / rating) to narrow results.
- Click "Add to cart" to add an item; open the cart to view and change quantities.
- Cart contents persist across page reloads via localStorage.
- The checkout flow is a placeholder — extend it to integrate payments/backend.

## Project structure (example)

Adjust these paths if your repository layout differs.

- index.html — entry page
- css/
  - styles.css
- js/
  - main.js — application bootstrap and event wiring
  - products.js or data/products.json — sample product data
  - cart.js — cart management (add/remove/persist)
  - ui.js — UI helpers, renderers
- assets/
  - images/ — product images, icons
- README.md

If your repository layout differs, update this section to match.

## Customizing products & data

- If products are defined in a JavaScript array (e.g., `products.js`), edit that file to add/remove products.
- If using `data/products.json`, update the JSON and ensure the fetch path in your code matches.
- For images, place them under `assets/images/` and update product image paths accordingly.

## Deployment

- GitHub Pages: Push to `main` (or `gh-pages`) and enable Pages for the repo.
- Netlify / Vercel: Connect the repo and deploy as a static site (no build step required unless you add one).
- Any static host that serves files over HTTPS will work.



## Contact

GitHub: [thatoneluckyguy](https://github.com/thatoneluckyguy)

---

