# Antonio Burgov — CV / Portfolio Website

A personal CV & portfolio site built with plain **HTML & CSS** (plus a little vanilla
JavaScript for interactivity). No build step, no dependencies — just open and go.

---

## 📂 What's inside

```
Antonio-CV-Website/
├── index.html                     ← the website (open this)
├── projects/                      ← live, testable project demos
│   ├── food-store/index.html      → FoodGo — food delivery mockup
│   ├── leasing/index.html         → ЛизингПро — digital leasing prototype
│   └── rpg-bulgaria/index.html    → Легенди на България — history quiz RPG
└── _design-explorations/          ← early design options (A / B / C) — reference only
```

The `projects/` folder powers the **"Try it live"** viewer on the site, with a
Desktop / Tablet / Mobile toggle so visitors can test each design responsively.

---

## ▶️ How to view it

**Easiest:** double-click `index.html` — it opens in your browser.

**Recommended (so the live demos load reliably):** run a tiny local server from this folder:

```bash
# Option 1 — Python (already on macOS)
python3 -m http.server 8000

# Option 2 — Node
npx serve
```

Then open **http://localhost:8000** in your browser.

---

## 🖼️ Add your photo

1. Make a PNG of yourself with a **transparent background** (free: https://remove.bg).
2. Save it as **`photo.png`** in this folder (next to `index.html`).
3. In `index.html`, find the `<!-- ADD YOUR PHOTO -->` comment in the hero section,
   delete the `<div class="photo-ph">…</div>` placeholder, and uncomment:
   ```html
   <img src="photo.png" alt="Antonio Burgov">
   ```

---

## 🔗 Wire up the real project demos

When you deploy a real project (e.g. the Angular food store), open `index.html`,
find the `demos` object near the bottom in `<script>`, and paste the live URL:

```js
const demos = {
  food:    { title: 'FoodGo — Food Delivery',      url: 'https://your-live-app.com' },
  leasing: { title: 'ЛизингПро — Digital Leasing', url: 'projects/leasing/index.html' },
  rpg:     { title: 'Легенди на България',          url: 'projects/rpg-bulgaria/index.html' }
};
```

The viewer will embed it automatically — desktop/tablet/mobile toggle included.

---

## 🚀 How to host it (free)

All three options are free and take a few minutes:

### GitHub Pages
1. Create a GitHub repo and push this folder.
2. Repo **Settings → Pages →** Source: `main` branch, `/root`.
3. Your site goes live at `https://<username>.github.io/<repo>`.

### Vercel
1. Go to https://vercel.com → **Add New → Project**.
2. Import the repo (or drag-and-drop this folder).
3. Framework preset: **Other**. Deploy. Done.

### Netlify
Just **drag this whole folder** onto https://app.netlify.com/drop — instant live URL.

---

## ✏️ Editing content

Everything is in `index.html` — it's organized top to bottom by section
(hero, what I do, about, projects, skills, experience, contact). Each section is
clearly commented. Colors live in the `:root { … }` block at the top of the `<style>`.

The site also includes a **dark-mode toggle**, scroll animations, and a sticky nav.

---

*Built with Claude Code · Sofia, Bulgaria · 2026*
