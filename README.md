# Local Store E-commerce Platform — Cubbon Corner Market

Task-03 · ProDigy InfoTech Web Development Internship

A single-page e-commerce website for a fictional local grocery store
("Cubbon Corner Market", modelled on a neighbourhood store in Bengaluru),
letting customers browse products, add them to a cart, and check out —
plus order tracking, reviews, and customer support.

## How to run

No installation, server, or build step needed — it's one self-contained
HTML file.

1. Download `index.html`.
2. Open it in any modern browser (Chrome, Firefox, Edge, Safari).
3. Start shopping.

## Core features (required by the brief)

- **Product listings** — 12 products across 5 categories (Bakery, Dairy,
  Produce, Snacks, Beverages, Grocery, Home), each with an image (icon-based
  so the file stays fully self-contained/offline), name, description, and
  price.
- **Browse & purchase** — add to cart, adjust quantities, remove items, and
  complete checkout with a delivery details form (name, phone, address).
- **Shopping cart** — slide-out cart drawer with live subtotal, delivery fee
  (free above ₹999), and total; persists across page reloads via
  `localStorage`.

## Optional features included

- **Order tracking** — checkout generates an order ID (e.g. `CCM-1042`);
  the "Track order" tab looks it up and shows a delivery timeline (Placed →
  Packed → Out for delivery → Delivered).
- **User reviews** — each product has a "reviews" link opening its rating
  and comments, with a form to add a new star rating + review.
- **Customer support** — an FAQ accordion plus a contact form with
  validation and a confirmation message.
- **Sort & filters** — category filter chips, a text search box, and a sort
  dropdown (price low–high, price high–low, rating).

## Validation

- Checkout requires a valid name, a 10-digit phone number, and a complete
  address before an order is placed.
- The support form checks for a name, a valid email format, and a non-empty
  message.
- Reviews require a star rating, a name, and a short comment.

## Data storage

Cart contents, placed orders, and reviews are stored in the browser's
`localStorage`, so they survive a page refresh but live only on the device
that placed them. There's no real backend, payment gateway, or database —
this is a front-end demo suited to a course/internship submission, not a
production storefront.

**Note on going to production:** a real version of this store would need a
backend (e.g. Node.js/Express or Django) with a product database, a
real payment gateway, server-side order storage, and authenticated user
accounts — so orders and reviews aren't just local to one browser.

## Tech stack

- HTML5, CSS3 (custom properties, responsive grid/flex layout, dark mode)
- Vanilla JavaScript (no frameworks or build step)
- Google Fonts (Fraunces / Work Sans)

## File structure

```
local-store-ecommerce/
├── index.html   # the entire application
└── README.md    # this file
```
