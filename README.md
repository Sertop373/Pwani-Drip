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
```

### Connect real M-Pesa payments
Replace the `placeOrder()` function with a real API call to [Pesapal](https://pesapal.com) or [Flutterwave](https://flutterwave.com) — both support M-Pesa STK push in Kenya.

---

## 🌐 Deploy to GitHub Pages — Step by Step

### Step 1 — Create a GitHub account
Go to [github.com](https://github.com) and sign up if you haven't already.

---

### Step 2 — Create a new repository
1. Click the **+** button (top right of GitHub) → **New repository**
2. Set the repository name to: `pwani-drip`
3. Set visibility to **Public**
4. Leave everything else unchecked
5. Click **Create repository**

---

### Step 3 — Rename your file to `index.html`
Before uploading, rename `pwani_drip.html` to **`index.html`** on your computer.
GitHub Pages looks for `index.html` as the entry point.

---

### Step 4 — Upload your files
1. In your new empty repo, click **uploading an existing file** (the link in the middle of the page)
2. Drag and drop both files:
   - `index.html`
   - `README.md`
3. In the commit message box type: `Initial commit — Pwani Drip store`
4. Click **Commit changes**

---

### Step 5 — Enable GitHub Pages
1. In your repo, click **Settings** (top tab)
2. In the left sidebar, scroll down and click **Pages**
3. Under **Source**, select **Deploy from a branch**
4. Set **Branch** to `main` and folder to `/ (root)`
5. Click **Save**

---

### Step 6 — Wait 1–2 minutes, then visit your live URL

GitHub Pages will build and deploy your site. Your live URL will be:

```
https://YOUR-GITHUB-USERNAME.github.io/pwani-drip/
```

Refresh the Pages settings tab after a minute — GitHub will show you the exact link when it's ready.

---

### Step 7 — Add the links to your portfolio

Once live, open `portfolio_app.py` and update the Pwani Drip project entry:

```python
"live": "https://YOUR-USERNAME.github.io/pwani-drip/",
"code": "https://github.com/YOUR-USERNAME/pwani-drip",
```

---

## 🗺️ Roadmap

- [ ] Connect real M-Pesa API (Pesapal / Flutterwave)
- [ ] Product search bar
- [ ] User accounts and order history
- [ ] Admin panel for inventory management
- [ ] WhatsApp notification on new orders
- [ ] Backend with Node.js + MongoDB

---

## 👤 Author

Built by a developer from Mombasa, Kenya 🇰🇪

---

## 📄 License

Open source — [MIT License](LICENSE)
