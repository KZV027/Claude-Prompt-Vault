# 🔮 Claude Prompt Vault

> The Best Claude Prompts. Instantly Copy. Instantly Build.

A premium, single-file web app for browsing, copying, and downloading curated Claude AI prompts and skill repositories.

## ✨ Features

- **114 curated prompts** from [AI Hustle Guy](https://aihustleguy.com)
- **5 real GitHub skill repos** — travisvn, BehiSecc, JayZeeDesign, K-Dense-AI, AgriciDaniel
- **Unified search** — search prompts and skills simultaneously
- **Segmented filter** — All / Prompts / Skills toggle with live counts
- **Category filters** — 12 prompt categories
- **Copy to clipboard** — one click copy
- **Download as .txt** — save any prompt locally
- **Full prompt modal** — read and copy the complete prompt text
- **Bookmark** — save prompts in-session
- **Newsletter CTA** — email capture
- **Fully responsive** — mobile, tablet, desktop
- **Zero dependencies** — single HTML file, no build step

## 🚀 Deploy in 30 seconds

### Vercel
1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) → New Project → Import your repo
3. No config needed — deploys automatically

### Netlify
1. Go to [netlify.com](https://netlify.com) → Add new site → Deploy manually
2. Drag and drop the `index.html` file into the deploy zone
3. Done — live in seconds

### GitHub Pages
1. Push to GitHub
2. Settings → Pages → Source: `main` branch, `/ (root)`
3. Your site will be live at `https://yourusername.github.io/repo-name`

## 🗂 Project Structure

```
claude-prompt-vault/
├── index.html      ← Entire app (HTML + CSS + JS, self-contained)
└── README.md       ← This file
```

## 🎨 Design

- **Fonts:** Fraunces (display) + DM Sans (body)
- **Palette:** Warm parchment (#F5EDE0) + Claude orange (#CC785C)
- **Style:** Premium SaaS — inspired by Linear, Vercel, Stripe

## ➕ Adding More Prompts

Open `index.html` and find `const prompts = [` in the `<script>` tag.

Add a new object following this shape (next available ID: 127):

```js
{
  id: 28,                          // unique number
  title: "Your Prompt Title",
  category: "writing",             // see category list below
  author: "Author Name",
  preview: "Short description shown on the card (1–2 sentences)",
  full: "The complete prompt text goes here."
}
```

**Available categories:**
`writing` · `content-strategy` · `social-media` · `linkedin` · `twitter` · `youtube` · `video-content` · `short-video` · `repurposing` · `content-ideas` · `seo` · `coding` · `marketing` · `research` · `productivity` · `analysis` · `creative`

## ➕ Adding More Skills

Find `const skills = [` and add:

```js
{
  name: "username/repo-name",
  desc: "Description of what this skill does.",
  icon: "🔧",
  tag: "Category",
  github: "https://github.com/username/repo-name"
}
```

## 📄 License

MIT — free to use, modify, and distribute.

---

Built with ❤️ using Claude AI
