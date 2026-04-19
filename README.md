# 🌐 Chandra Mohan — Cyber Portfolio

> Personal portfolio website of **Chandra Mohan** — Full Stack Developer, Cybersecurity Enthusiast & CSE (Data Science) student from Vijayawada, Andhra Pradesh, India.

---

## 📌 Live Preview

Open `index.html` directly in any modern browser — **no build step, no server required.**

---

## 🗂️ Project Structure

```
portfolio/
│
├── index.html          # Single-file portfolio (HTML + CSS + JS all-in-one)
└── README.md           # This file
```

Everything lives inside one self-contained `index.html` file — no frameworks, no bundlers, no dependencies to install.

---

## ✨ Features

### 🎨 Design & Theme
- **Void + Purple + Gold** dual-accent color system
- Dark background (`#07050f`) with layered depth
- Gold shimmer animation on the hero heading
- Glowing progress bars, stat counters, and section highlights
- Scanline overlay for a subtle cyberpunk aesthetic

### 🌌 3D Animated Background (Three.js)
- Dense **starfield** with colored depth particles
- **Neural-network node system** — 120 animated nodes with live connecting lines
- **Floating wireframe geometry** — icosahedra, octahedra, tori (purple + gold)
- **Drift particles** rising upward with glow
- **Perspective grid** pulsing at the base
- **Mouse-driven parallax** camera movement

### 🌊 Additional Animations
- **Aurora waves** — 4 layered sine-wave gradients flowing behind the scene
- **Floating orbs** — 3 CSS radial-gradient orbs that drift and pulse
- Typewriter role cycling effect
- Scroll fade-in via IntersectionObserver
- Tab pause/resume on visibility change (battery-friendly)

### 📱 Responsive Design
- Fully responsive across all screen sizes
- **Hamburger menu** on mobile/tablet (≤ 960px) with slide-open drawer
- Single-column layouts on small screens
- Stacked buttons and scaled typography on mobile

### 🔐 Security
| Header / Feature | Value |
|---|---|
| `X-Content-Type-Options` | `nosniff` |
| `X-Frame-Options` | `DENY` |
| `Referrer-Policy` | `strict-origin-when-cross-origin` |
| `Content-Security-Policy` | Restricts scripts, styles, images to trusted CDNs only |
| External links | `rel="noopener noreferrer"` on all `target="_blank"` links |
| Three.js CDN | SRI hash integrity check |

### 🧩 Sections
| # | Section | Description |
|---|---|---|
| 01 | **Hero** | Name, animated role typewriter, meta chips, CTA buttons, 3D HUD visual |
| 02 | **About** | Profile card, info table, skill progress bars, tags |
| 03 | **Skills** | 6 category cards — Full Stack, Cybersecurity, AI/DS, Systems, Creative |
| 04 | **Projects** | Tabbed view — Full Stack, Cybersecurity, Upcoming |
| 05 | **Journey** | Education, internship, hackathon milestones |
| 06 | **Contact** | Direct-link cards for Email, GitHub, LinkedIn, YouTube |

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 (semantic) |
| Styling | CSS3 — custom properties, grid, flexbox, animations |
| Scripting | Vanilla JavaScript (ES5-safe) |
| 3D Graphics | [Three.js r128](https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js) |
| Fonts | Google Fonts — Syne, DM Sans, JetBrains Mono |
| Icons | SVG inline (GitHub), emoji icons |
| Favicon | Inline SVG data URI — no external file needed |

**Zero npm. Zero build tools. Zero frameworks.**

---

## 🚀 Deployment

### Option 1 — GitHub Pages (recommended)
1. Push `index.html` and `README.md` to a GitHub repository
2. Go to **Settings → Pages**
3. Set source to `main` branch, root `/`
4. Your site will be live at `https://<your-username>.github.io/<repo-name>/`

### Option 2 — Netlify Drop
1. Go to [netlify.com/drop](https://app.netlify.com/drop)
2. Drag and drop the `index.html` file
3. Get an instant live URL

### Option 3 — Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in the project folder
3. Follow the prompts — done

### Option 4 — Local
Just double-click `index.html` or open it in any browser. No server needed.

---

## 🎨 Customization Guide

### Update Personal Info
All content is inside `index.html`. Search for these and replace:

| What to change | Search for |
|---|---|
| Your name | `Chandra Mohan` |
| Your location | `Vijayawada, Andhra Pradesh` |
| Your email | `chandramohannmp@gmail.com` |
| GitHub profile | `chandramohann-4510` |
| LinkedIn profile | `chandra-mohan-50a7a03b2` |
| Typewriter roles | Array inside `(function()` → `var phrases = [...]` |

### Swap Colors
CSS variables are at the top of the `<style>` block:
```css
:root {
  --g1: #c9a227;   /* primary gold  — change this */
  --g2: #e8c44a;   /* bright gold   — change this */
  --p1: #b06ef3;   /* main purple   — change this */
  --p2: #7c3aed;   /* deep violet   — change this */
}
```

### Add a New Project Card
Copy a `.proj-card` block inside the appropriate `#tab-fullstack`, `#tab-cyber`, or `#tab-upcoming` div and update the title, description, and tech tags.

### Add a New Journey Entry
Copy a `.journey-card` block inside `.journey-grid` and update the date, title, organisation, and description.

---

## 📊 Stats Displayed

| Metric | Value |
|---|---|
| Hackathons participated | 5 |
| Runner-up finishes | 2 🥈 |
| Projects built | 7+ |
| Internships | 1 |

---

## 🔗 Connect

| Platform | Link |
|---|---|
| 📧 Email | [chandramohannmp@gmail.com](mailto:chandramohannmp@gmail.com) |
| 🐙 GitHub | [github.com/chandramohann-4510](https://github.com/chandramohann-4510) |
| 💼 LinkedIn | [linkedin.com/in/chandra-mohan-50a7a03b2](https://www.linkedin.com/in/chandra-mohan-50a7a03b2) |
| ▶️ YouTube | Coming Soon |

---

## 📄 License

This portfolio is **personal and open-source for inspiration.**
Feel free to use it as a reference or starting point — just don't copy it wholesale and claim it as your own.

---

> Built with passion · Full Stack · Cybersecurity · AI · 2026
