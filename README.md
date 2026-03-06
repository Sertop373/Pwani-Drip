# 🌊 Pwani Drip — Mombasa Streetwear Store

A fully functional, single-file e-commerce storefront built for a Mombasa-based streetwear brand. Clean dark luxury aesthetic with amber accents, custom cursor, 3D product card tilt, and a complete shopping flow from browsing to M-Pesa checkout.

---

## 🖥️ Live Demo

> **[View Live Site](#)** · **[GitHub Repository](#)**
> *(Replace `#` with your deployed URL and repo link)*

---

## ✨ Features

- **6 fully working pages** — Home, Shop, Product Detail, Cart, Checkout, About
- **8 products** across Tees, Hoodies, and Accessories
- **Live cart** — add, remove, update quantities in real time
- **Promo code** — `PWANI10` applies a 10% discount
- **M-Pesa checkout flow** — STK push mockup, card, and pay-on-delivery options
- **Custom glowing cursor** with context labels (View, Add, Shop, Explore)
- **3D card tilt** — product cards rotate in perspective on hover
- **Staggered hero animations** — sequential entrance on page load
- **Infinite marquee** — pauses on hover
- **Category filtering** — All / Tees / Hoodies / Accessories
- **Toast notifications** — non-intrusive feedback on cart actions
- **Noise/grain texture overlay** — subtle film grain for depth
- **Fully responsive** — mobile, tablet, and desktop
- **Zero dependencies** — pure HTML, CSS, and vanilla JavaScript

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Markup | HTML5 |
| Styling | CSS3 (custom properties, grid, flexbox, animations) |
| Logic | Vanilla JavaScript (ES6+) |
| Fonts | Bebas Neue, Outfit, Space Mono (Google Fonts) |
| Images | Unsplash CDN (replace with real product photos) |
| Payments | M-Pesa mockup — integrate Pesapal or Flutterwave for production |

---

## 📁 Project Structure

```
pwani-drip/
│
├── index.html      # Entire app — all 6 pages in one file
└── README.md       # You are here
```

Single-file build — ideal for portfolio demos and easy deployment on any static host.

---

## 🚀 Run Locally

No installs needed. Just open the file:

```bash
# Option 1 — double-click index.html in your file manager

# Option 2 — serve with Python (avoids any CORS issues)
python3 -m http.server 3000
# Then visit http://localhost:3000
```

---

## 🛒 Shopping Flow

```
Browse → Add to Bag → Cart → Promo Code → Checkout → M-Pesa → Done
```

- Promo code **`PWANI10`** = 10% off any order
- Free shipping on orders over **KSh 3,000**

---

## 🎨 Customisation

### Add or edit a product
Find the `PRODS` array in `index.html` and follow this structure:

```javascript
{
  id: 9,
  name: "New Product Name",
  cat: "Tees",              // Tees | Hoodies | Accessories
  price: 2500,              // Price in KSh
  orig: 3000,               // Strike-through price (null if no sale)
  img: "https://...",       // Main image URL
  imgs: ["https://..."],    // All gallery images
  badge: "New",             // "New" | "Sale" | null
  sizes: ["S","M","L","XL"],
  mat: "220gsm Cotton",
  feat: true,               // true = appears on homepage grid
  desc: "Product description."
}



