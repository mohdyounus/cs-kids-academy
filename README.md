# 🤖 CS Kids Academy

An interactive Computer Science learning website for kids (~10 years old).  
Self-contained — just one `index.html` file, **no build step required**.

## 🚀 Run Locally

```
Open cs-kids-academy/index.html in any modern browser.
```

Or with a local server (avoids CORS on the translate API):

```bash
# Python
python -m http.server 8080

# Node
npx serve .
```

Then visit http://localhost:8080

## ✨ Features

| Feature | Details |
|---------|---------|
| 8 chapters | Computer parts, binary, algorithms, coding, internet, safety, loops, AI |
| Progress tracking | `localStorage` — survives page refresh |
| Per-chapter quiz | Must pass before "Mark Complete" unlocks |
| Confetti 🎉 | Triggers when all chapters are complete |
| Printable certificate | Enter your name → print |
| Read Aloud | `SpeechSynthesis` API — works offline |
| Translation | LibreTranslate (English → Hindi / Urdu) |
| RTL support | Urdu flips layout automatically |
| Responsive | Works on phone, tablet, desktop |

## 🌐 Translation API

The site uses the **LibreTranslate** public demo (`https://libretranslate.com/translate`).

- No API key needed for occasional use
- For production, self-host LibreTranslate or use the paid tier
- Replace `LIBRE_URL` at the top of the `<script>` section with your self-hosted URL

## 🌍 Deploy for Free

### GitHub Pages (easiest)

```bash
git init
git add .
git commit -m "CS Kids Academy"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/cs-kids-academy.git
git push -u origin main
```
Then enable GitHub Pages in repository Settings → Pages.

### Netlify / Vercel / Cloudflare Pages

Drag & drop the `cs-kids-academy` folder into any of these services — no build step needed.

## 📁 Structure

```
cs-kids-academy/
└── index.html   ← entire website (HTML + CSS + JS)
└── README.md
```
