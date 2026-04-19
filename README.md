# 🚀 Chandra Mohan — Cyber Portfolio

> A fully animated, 3D immersive personal portfolio built with vanilla HTML, CSS, and Three.js.
> **Void + Purple** cyberpunk aesthetic — professional, futuristic, and visually dramatic.

---

## 👤 About

**Chandra Mohan** | CSE (Data Science) · 2nd Year | Vijayawada, Andhra Pradesh, India

- 📧 chandramohannmp@gmail.com
- 💼 [LinkedIn](https://www.linkedin.com/in/chandra-mohan-50a7a03b2)
- 🐙 [GitHub](https://github.com/chandramohann-4510)
- 📍 Vijayawada, Andhra Pradesh, India
- 🟢 **Open for Internships** in Cybersecurity / Full Stack / AI / Data Science

---

## ✨ Features

### 🌐 5-Layer 3D Animated Background (Three.js)

| Layer | What it does |
|-------|-------------|
| **Layer 1 — Starfield** | 1,800 deep-space background stars in purple tones |
| **Layer 2 — Neural Network** | 120 animated nodes that move, bounce, and connect with glowing lines when close |
| **Layer 3 — Drift Particles** | 320 glowing particles that drift upward continuously |
| **Layer 4 — 3D Shapes** | 8 floating wireframe icosahedrons, octahedrons, and tori that rotate, float, and pulse |
| **Layer 5 — Grid Plane** | Perspective grid at the base for depth |

- Mouse-driven parallax camera — the entire 3D scene reacts to your cursor
- All rendered live in WebGL via Three.js r128 with SRI integrity hash for security
- Tab-visibility detection: animation pauses when tab is hidden (saves GPU/battery)

### 💻 Visual Design
- **Void + Purple theme** — ultra-dark `#07050f` base with `#b06ef3` purple, `#7c3aed` violet, `#e879f9` fuchsia, `#a78bfa` lavender accents
- **Custom fonts** — Syne (headings), DM Sans (body), JetBrains Mono (code labels)
- **No custom cursor** — uses default system cursor for clean UX
- **No scroll lines** — removed all decorative vertical scroll indicators
- **Typewriter effect** cycling through roles in the hero section
- **Scroll-triggered fade-in** for every section
- **Animated progress bars** that fill on scroll into view

### 📄 Sections

| # | Section | Description |
|---|---------|-------------|
| 01 | **About** | Profile card + biography + skill progress bars + interest tags |
| 02 | **Skills** | 6 skill category cards with color-coded tech pills |
| 03 | **Projects** | Modern tab layout — Full Stack / Cybersecurity / Upcoming |
| 04 | **Journey** | Internship + education (2024–2028 corrected) + hackathon banner |
| 05 | **Contact** | Email, GitHub, LinkedIn, YouTube links |

---

## 🛠️ Technologies Used

| Category | Tech |
|----------|------|
| Structure | HTML5 (single file) |
| Styling | CSS3 (Custom Properties, Grid, Flexbox, Keyframe Animations) |
| 3D Engine | [Three.js r128](https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js) |
| Fonts | [Syne](https://fonts.google.com/specimen/Syne), [DM Sans](https://fonts.google.com/specimen/DM+Sans), [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) via Google Fonts |
| Deployment | Any static host (GitHub Pages, Netlify, Vercel) |

---

## 📁 Project Structure

```
portfolio/
├── index.html          ← Single-file portfolio (all CSS + JS embedded)
└── README.md           ← This file
```

> The entire portfolio is a **single HTML file** — zero build steps, zero dependencies to install.
> Just open `index.html` in a browser and it works.

---

## 🚀 Getting Started

### Option 1 — Open Locally
```bash
# Clone or download the repo
git clone https://github.com/chandramohann-4510/portfolio.git

# Open directly in your browser
open index.html
# or on Windows:
start index.html
```

### Option 2 — Deploy to GitHub Pages
```bash
git init
git add .
git commit -m "Initial portfolio commit"
git branch -M main
git remote add origin https://github.com/chandramohann-4510/portfolio.git
git push -u origin main
# Then: Settings → Pages → Source: main branch → / (root)
# Live at: https://chandramohann-4510.github.io/portfolio
```

### Option 3 — Deploy to Netlify (Free, Recommended)
1. Go to [netlify.com](https://netlify.com)
2. Drag and drop the `index.html` file
3. Your site is instantly live

### Option 4 — Deploy to Vercel
```bash
npm install -g vercel
vercel --name chandra-mohan-portfolio
```

---

## ✏️ Customisation Guide

### Update Personal Info

| Field | Search For | Replace With |
|-------|-----------|--------------|
| Email | `chandramohannmp@gmail.com` | Your email |
| GitHub | `chandramohann-4510` | Your GitHub username |
| LinkedIn | `chandra-mohan-50a7a03b2` | Your LinkedIn ID |
| Location | `Vijayawada` | Your city |

### Change Color Theme
Edit the CSS variables at the top of the `<style>` block:
```css
:root {
  --p1: #b06ef3;   /* Main purple */
  --p2: #7c3aed;   /* Deep violet */
  --p3: #e879f9;   /* Fuchsia accent */
  --p4: #a78bfa;   /* Soft lavender */
}
```

### Add a New Project
Find the comment `<!-- FULL STACK -->` and copy a `.proj-card` block:
```html
<div class="proj-card">
  <div class="proj-card-top-line"></div>
  <div class="proj-header">
    <div class="proj-icon-box">🔧</div>
    <span class="proj-badge pb1">Full Stack</span>
  </div>
  <div class="proj-title">Your Project Name</div>
  <p class="proj-desc">Your project description here.</p>
  <div class="proj-tech">
    <span class="tech-tag">Tech 1</span>
    <span class="tech-tag">Tech 2</span>
  </div>
</div>
```

### Adjust 3D Particle Intensity
In the JavaScript section, modify these values:

```js
var NODE_COUNT = 120;    // number of neural network nodes (reduce for better performance)
var MAX_DIST   = 18;     // max distance for connection lines (reduce for fewer lines)
var driftCount = 320;    // number of upward-drifting glow particles
var starCount  = 1800;   // background starfield density
```

### Update Skill Progress Bars
Find `data-width="82"` and change the number (0–100):
```html
<div class="prog-fill pf1" data-width="82"></div>
```

---

## 📱 Responsive Design

| Breakpoint | Behaviour |
|-----------|-----------|
| ≥ 960px | Full layout — 2-column hero with HUD orbit visual |
| < 960px | Single column — orbit HUD hidden, nav links hidden |
| < 600px | Compact padding for small phones |

---

## 🛡️ Security Notes

- ✅ **No external API keys** used or exposed
- ✅ **No backend** — fully static, no server-side vulnerabilities
- ✅ **External links** use `rel="noopener noreferrer"` (prevents tab-napping)
- ✅ **Three.js** loaded from trusted CDN with **SRI integrity hash** (prevents CDN tampering)
- ✅ **Google Fonts** loaded via HTTPS
- ✅ **No `eval()`** — zero dangerous JavaScript patterns
- ✅ **No `innerHTML`** with user-controlled data
- ✅ **No cookies or localStorage** used
- ✅ **No form submission** — contact is via direct links only
- ✅ **Security meta headers** included: `X-Content-Type-Options`, `X-Frame-Options: DENY`, `Referrer-Policy`
- ✅ **Tab visibility API** — 3D animation pauses when tab is hidden

### Recommended: Add CSP Header on Deployment
When hosting on Netlify or Vercel, add this Content Security Policy:
```
Content-Security-Policy: default-src 'self'; script-src 'self' 'unsafe-inline' cdnjs.cloudflare.com; style-src 'self' 'unsafe-inline' fonts.googleapis.com; font-src fonts.gstatic.com; img-src 'self' data:;
```

**Netlify** — create a `_headers` file in the same folder:
```
/*
  Content-Security-Policy: default-src 'self'; script-src 'self' 'unsafe-inline' cdnjs.cloudflare.com; style-src 'self' 'unsafe-inline' fonts.googleapis.com; font-src fonts.gstatic.com;
  X-Frame-Options: DENY
  X-Content-Type-Options: nosniff
```

---

## 📸 Portfolio Sections Overview

### Hero Section
- Typewriter cycling through 6 roles
- 4-ring HUD orbital animation with 3 orbiting glowing nodes
- Meta chips: location, degree, specialization
- CTA buttons: View Projects & Contact Me
- Stats bar: 8 Hackathons · 2 Runner-Up · 7+ Projects · 1 Internship

### About Section
- Profile card with avatar, info grid, live status indicator
- Biography covering full stack, cybersecurity, and content creation
- Animated skill progress bars (scroll-triggered)
- Interest/passion tags

### Skills Section (6 categories)
1. **Programming Languages** — C, Python, JavaScript, TypeScript, HTML5, CSS3
2. **Full Stack Web Dev** — React, Next.js, Node.js, Express, MongoDB, Tailwind
3. **Cybersecurity** — Linux, Steganography, Cryptography, Networking, JetPhisher, Google Dorks, OSINT, Phishing Detection, SOC
4. **AI & Data Science** — AI Agents, Vibe Coding, API Integration, ML, Computer Vision
5. **Systems & Tools** — OS, Git, Kali Linux, Wireshark, VS Code, Postman
6. **Creative & Content** — Video Editing, Content Creation, UI/UX Design

### Projects Section (Modern Tab Layout)
**Full Stack:**
- Wildlife Species Detection (AI + Computer Vision)
- College Smart Attendance System (Live Cam + Face Recognition)
- Smart Exam Planner (React.js Frontend)

**Cybersecurity:**
- Advanced Steganography Tool (Images, Video, Audio)
- CyberVerse Security Toolkit (7+ integrated tools)

**Upcoming:**
- Smart Mentoring System
- Anti-Phishing Website Blocker
- Advanced Cyber Tools Suite

### Journey Section
- Ethical Hacking & Data Security Internship — Supraja Technologies (2024)
- B.Tech CSE (Data Science) — Vijayawada · **2024–2028** ✅ Updated
- Hackathon Banner: 8 attended, 2 Runner-Up finishes

### Contact Section
- Email, GitHub, LinkedIn, YouTube (Coming Soon)

---

## 📜 License

This portfolio is personal work by **Chandra Mohan**. You are welcome to use it as inspiration or a template — please give credit if you fork it.

---

## 🌟 Acknowledgements

- 3D background powered by [Three.js](https://threejs.org/)
- Fonts by [Google Fonts](https://fonts.google.com/)
- Design — original Void + Purple concept by Chandra Mohan

---

<p align="center">
  Built with ❤️ by <strong>Chandra Mohan</strong> · Vijayawada, India · 2025
</p>
<p align="center">
  <em>Full Stack · Cybersecurity · AI · Content Creation</em>
</p>
