# Riz Talks Finance

Personal website for [riztalksfinance.com](https://riztalksfinance.com) — a personal finance brand helping early-to-mid career professionals build financial security.

---

## Live site

Hosted via GitHub Pages / Vercel at: **riztalksfinance.com**

---

## What this is

A single-page personal brand website. One HTML file, no framework, no build step. Designed to be hosted on GitHub Pages or Vercel and pointed at a custom domain.

---

## Structure

```
index.html       ← The entire website. Everything is in here.
README.md        ← This file
your-photo.jpg   ← Add your photo here (see setup below)
```

---

## Sections

| Section | What it does |
|---|---|
| Hero | Headline, bio, stats, photo, two CTAs |
| Logos | Career background (Careem, Bolt, Wise, Motive, Soch) |
| Problems | The 3 financial problems the brand solves |
| About | Story, credentials, audience breakdown, stats |
| Work With Me | 1:1 Coaching, Happy Money course, Community |
| Content | The 5 weekly content pillars |
| Testimonials | Dilawar Ali and Abbas Rizvi with LinkedIn links |
| Newsletter | Kit and Substack subscribe links |
| Channels | All social platforms linked |
| CTA | Final WhatsApp + Instagram push |
| Footer | Nav links |

---

## Setup

### 1. Add your photo

The hero section currently shows a placeholder. To add your photo:

1. Add your photo file to the repo root — name it `photo.jpg` (or any name you prefer)
2. In `index.html`, find this block:

```html
<div class="hero-photo-bg">
  <div class="ph-icon">👤</div>
  <p>Your photo here</p>
</div>
```

3. Replace it with:

```html
<img src="photo.jpg" style="width:100%;height:100%;object-fit:cover;object-position:center top;display:block;border-radius:0 0 0 16px"/>
```

---

### 2. Deploy to GitHub Pages

1. Push `index.html` (and your photo if you have one) to a GitHub repo
2. Go to repo **Settings → Pages**
3. Set Source to **Deploy from a branch → main → / (root)**
4. GitHub will give you a live URL within 60 seconds

---

### 3. Deploy to Vercel (recommended)

1. Push the repo to GitHub
2. Go to [vercel.com](https://vercel.com) → New Project → Import your GitHub repo
3. Vercel auto-detects a static site — click Deploy
4. Your site is live at `yourname.vercel.app`

To connect `riztalksfinance.com`:
- In Vercel: Settings → Domains → Add `riztalksfinance.com`
- In your domain registrar: point the DNS to Vercel's nameservers (Vercel gives you exact instructions)

---

## Brand

| Token | Value |
|---|---|
| Primary font | DM Sans (Google Fonts) |
| Navy | `#091D36` |
| Orange | `#DF643A` |
| Light Blue | `#7A97CA` |
| White | `#FFFFFF` |

---

## Links

| Platform | URL |
|---|---|
| Instagram | instagram.com/RizTalksFinance |
| YouTube | youtube.com/@RizTalksFinance |
| LinkedIn | linkedin.com/in/RizTalksFinance |
| TikTok | tiktok.com/@RizTalksFinance |
| X | x.com/RizTalksFinance |
| Kit Newsletter | riztalksfinance.kit.com/newsletter |
| Substack | riztalksfinance.substack.com |
| WhatsApp | wa.me/+37253890745 |
| Soch | withsoch.com |

---

## Making changes

Everything is in `index.html`. The file is structured with clear HTML comments marking each section — search for `<!-- HERO -->`, `<!-- ABOUT -->`, `<!-- OFFER -->` etc. to find what you need to edit.

Colors and fonts are set as CSS variables at the top of the `<style>` block — change them once and they update everywhere:

```css
:root {
  --navy: #091D36;
  --orange: #DF643A;
  --blue: #7A97CA;
  --font: 'DM Sans', system-ui, sans-serif;
}
```

---

© 2025 Riz Talks Finance
