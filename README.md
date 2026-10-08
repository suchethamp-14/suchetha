# Suchetha — Software Engineer Portfolio

> A cyber-chic, high-performance software engineer portfolio engineered with dark tech glassmorphism aesthetics, retro 8-bit pixel art accents, synthesized Web Audio soundscapes, and zero external framework overhead.

---

## 🌟 Key Features & Components

### 1. Header & Navigation System
- **Responsive Layout:** Horizontal glassmorphic navigation bar on desktop; transformed into an accessible sliding vertical drawer on tablet and mobile viewports (`<=860px`).
- **Night / Day Mode:** Frosted glass toggle button supporting instant light and dark theme switching with persistence in `localStorage` and system theme auto-detection.
- **Synthesized 8-Bit SFX Engine:** Pure JavaScript Web Audio API oscillator synthesis generating retro chiptune audio feedback upon interactions (can be toggled on/off with persistent state).

### 2. Hero Section & Parallax Floating Chassis
- **Frosted Console:** Integrated system telemetry grid displaying core architectural competencies and availability.
- **3D Parallax Drift:** Floating portrait chassis bound to continuous vertical floating keyframes (`@keyframes floatParallax`) with breathing radial neon glow (`@keyframes pulseGlow`).
- **Interactive CTAs:** Primary and secondary action buttons with light-sweep shimmer pseudo-elements and smooth micro-elevations.

### 3. About Me Section
- **Profile Card Showcase:** High-resolution portrait chassis with geographic, availability, and role badges.
- **Narrative & Highlights:** Minimalist highlight cards featuring architecture philosophy, code craftsmanship, and personal tech interests.

### 4. Retro 8-Bit Skills Matrix
- **HUD Telemetry Matrix:** RPG-inspired status header detailing role levels, overclock indicators, and character attribute badges.
- **Category Cartridge Tabs:** Instant category switching between Languages, Frameworks, Cloud, and Systems.
- **Segmented XP Meters:** 8-bit pixel meters with animated fill transitions triggered via `IntersectionObserver` when scrolled into view.

### 5. Interactive Career & Education Timeline
- **Central Gradient Spine:** Neon cyan/indigo vertical track with glowing node icons.
- **Category Filtering:** Filter milestones across Career, Major Projects, Education, and System Achievements.
- **Rounded Cards:** Standardized border radii (`var(--radius-card)`) and multi-layered drop shadows (`var(--shadow-card)`).

### 6. Featured Software Projects & Blueprint Modals
- **Consistent Thumbnails:** Uniform 210px containers with macOS/terminal chrome bar, dynamic SVG topology illustrations, and hover zoom effects.
- **Detailed Inspection Modals:** Dynamic modal popups populated from a centralized data contract, detailing technical narratives, performance benchmarks, and tech tags.

### 7. System Architecture Video Showcase & Walkthrough
- **16:9 Responsive Chassis:** High-definition video player container with terminal chrome.
- **Live Canvas Simulation:** 60fps hardware-accelerated animated packet streams modeling Raft consensus quorum telemetry.
- **Playback Controls & Chapters:** Play/Pause toggle, seekable progress bar, and timestamp-based chapter navigation.

### 8. Testimonials & Peer Feedback Section
- **Client & Peer Feedback Cards:** Real-world quotes, role tags, star ratings, and quantifiable performance impact chips.
- **Category Navigation:** Filter testimonials by Managers, Peers, and Clients.

### 9. Interactive Glassmorphic Contact Form
- **Form Fields:** Name, Return Email, Transmission Subject, and Message textarea with cybernetic glow focus indicators.
- **Validation & Feedback:** Client-side validation with status alert banners and audio transmission feedback.
- **Fallback Channels:** Direct mailto triggers and tactile social pill buttons (GitHub, LinkedIn, Twitter).

### 10. Floating Cybernetic AI Terminal Chatbot Assistant
- **Accessible Widget:** Floating launcher button in the bottom right corner with pulse dot.
- **Contextual Copilot:** Automated assistant with natural query processing for skills, projects, experience, and contact.
- **Quick Action Chips:** Instant one-click chips for rapid information discovery and direct in-page anchor navigation.

---

## 🛠️ Technology Stack & Standards

- **Core Technologies:** Semantic HTML5, Vanilla CSS3 (Custom Properties & Design Tokens), Modern Vanilla JavaScript (ES6+).
- **Audio:** Web Audio API (Synthesized square and sine waves, zero external audio assets).
- **Typography:** Google Fonts (`Press Start 2P`, `Plus Jakarta Sans`, `Space Grotesk`, `JetBrains Mono`).
- **Icons & Graphics:** Clean inline SVGs and Unicode glyphs.
- **Performance:** Zero runtime dependencies or heavy JavaScript frameworks.

---

## 📱 Cross-Browser & Multi-Device Testing & Debugging Audit

The entire codebase has been reviewed and audited across modern browser engines (Blink/Chrome/Edge, Gecko/Firefox, WebKit/Safari) and viewports:

| Device Category | Viewport Width | Tested Browsers | Verification & Hardening Results |
| :--- | :--- | :--- | :--- |
| **Desktop / Widescreen** | 1280px &ndash; 1920px+ | Chrome, Edge, Firefox, Safari | ✅ Passed (Fluid CSS grid/flex, 60fps canvas simulation, contrast verified across Day/Night themes) |
| **Tablet / Small Laptop** | 860px &ndash; 1024px | Chrome, Safari iPadOS, Firefox | ✅ Passed (Reflowed telemetry grid, responsive blueprint modal, auto-adapting drawer navigation) |
| **Mobile (Standard)** | 480px &ndash; 860px | Safari iOS, Chrome Mobile | ✅ Passed (Vertical drawer navigation with backdrop, touch video toggle, dynamic chat sizing) |
| **Compact Mobile** | 320px &ndash; 480px | Chrome Mobile, Safari iOS | ✅ Passed (Horizontal overflow protection, touch targets >= 44px, chat max-height dynamic clamp) |

### 🔍 Hardened & Debugged Issues:
1. **Chat Widget Contrast Across Themes:** Enforced dedicated dark cyber-terminal tokens for `.chat-widget-window`, `.chat-input`, and `.chat-header` so input and messages remain 100% readable in both Day and Night modes.
2. **Chatbot Security (DOM XSS):** Implemented strict HTML entity escaping for user queries before rendering messages into the chat body.
3. **In-Chat Navigation on Mobile:** Added automatic minimization of the chat window when in-chat jump links (`#projects`, `#skills`, etc.) are clicked, preventing the chat window from obstructing view on mobile screens.
4. **Video Architecture Showcase (Touch & Mobile):** Added direct click-to-play/pause on the canvas element and container touch interaction for mobile/tablet browsers where hover pseudo-classes are inactive. Added compact controls padding for narrow mobile viewports.
5. **Mobile Viewport Stability:** Added `overflow-x: hidden` to root `html` and `body` to completely prevent horizontal panning/wobble from ambient drifting orbs.
6. **Contact Form Polish:** Ensured human-readable subject labels, client-side input sanitization, audio feedback on validation errors, and auto-scrolling to the transmission status banner on mobile.
7. **SEO & Social Previews:** Injected Open Graph (`og:*`), Twitter Card (`twitter:*`), and `theme-color` meta tags for professional previews on LinkedIn, Twitter, and messaging apps.
8. **Static Hosting Preparation:** Added `.nojekyll` configuration to project root for seamless asset loading on GitHub Pages.

---

## 🚀 Deployment Guide

### Option 1: Automated Deployment via GitHub Pages (Recommended)

This repository includes a pre-configured GitHub Actions workflow in [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml).

1. **Initialize Git & Push to GitHub:**
   ```bash
   git init
   git add .
   git commit -m "feat: initial release of cybernetic portfolio"
   git branch -M main
   git remote add origin https://github.com/<YOUR_USERNAME>/<YOUR_REPOSITORY>.git
   git push -u origin main
   ```

2. **Enable GitHub Pages:**
   - Go to your repository on GitHub.
   - Navigate to **Settings** &rarr; **Pages**.
   - Under **Build and deployment** &rarr; **Source**, select **GitHub Actions**.
   - The workflow will automatically trigger, build, and publish the portfolio to `https://<YOUR_USERNAME>.github.io/<YOUR_REPOSITORY>/`.

---

### Option 2: Manual Deployment via GitHub Pages (Branch Method)

1. Push all project files to the `main` branch.
2. In GitHub, go to **Settings** &rarr; **Pages**.
3. Under **Build and deployment** &rarr; **Source**, select **Deploy from a branch**.
4. Set the branch to `main` and folder to `/ (root)`.
5. Click **Save**. Your site will be live within 1–2 minutes.

---

### Option 3: Deploy to Vercel

1. Install the Vercel CLI or connect via GitHub:
   ```bash
   npm i -g vercel
   vercel
   ```
2. Or import the repository at [vercel.com/new](https://vercel.com/new).
3. Set Framework Preset to **Other**, leave build command blank, and deploy.

---

### Option 4: Deploy to Netlify

1. Drag and drop the project folder directly into [app.netlify.com/drop](https://app.netlify.com/drop).
2. Or connect your GitHub repository and select `main` as the production branch with no build command needed.

---

### Option 5: Local Development & Preview

To preview the portfolio locally using a lightweight HTTP server:

- **Using Python 3:**
  ```bash
  python -m http.server 8000
  ```
  Visit `http://localhost:8000` in your browser.

- **Using Node.js (`npx serve`):**
  ```bash
  npx serve .
  ```

---

## 📄 License & Credits

- Designed & Developed by **Suchetha** (Software Engineer).
- Built with semantic HTML5, modern CSS3, and vanilla JavaScript.
