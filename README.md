# 🏋️ IRON DISTRICT FITNESS — Premium Gym Website

> A premium, production-quality gym/fitness center website frontend demo built for **KSJ Technologies**. Designed to approach real gyms and fitness businesses as a sales demo.

---

## 🚀 Tech Stack

| Tool | Purpose |
|---|---|
| **React 19** | UI framework |
| **TypeScript** | Type safety |
| **Vite 8** | Build tool + dev server |
| **Tailwind CSS v4** | Utility-first styling |
| **Framer Motion** | Animations & transitions |
| **Lucide React** | Icon system |

---

## 📦 Getting Started

### Prerequisites
- Node.js 18+
- npm 9+

### Install & Run

```bash
# Install dependencies
npm install

# Start dev server
npm run dev

# Production build
npm run build

# Preview production build locally
npm run preview
```

---

## 🌐 Deploy to Vercel

### Option 1 — Vercel CLI

```bash
# Install Vercel CLI globally
npm i -g vercel

# From the project root
vercel

# Follow prompts — framework auto-detected as Vite
# Build command: npm run build
# Output dir: dist
```

### Option 2 — Vercel Dashboard (Recommended)

1. Push this repo to **GitHub / GitLab / Bitbucket**
2. Go to [vercel.com](https://vercel.com) → **Add New Project**
3. Import your repository
4. Vercel auto-detects Vite — no configuration needed
5. Click **Deploy**

> All settings are pre-configured in [`vercel.json`](./vercel.json).

---

## 🗂 Project Structure

```
src/
├── components/          # 29 fully-built sections
│   ├── Hero/            # Full-screen cinematic hero
│   ├── Programs/        # Training disciplines + modals
│   ├── Membership/      # Pricing matrix
│   ├── Trainers/        # Certified coach profiles
│   ├── Transformations/ # Before/after drag slider
│   ├── Facilities/      # Equipment tabs
│   ├── Schedule/        # Weekly class timetable
│   ├── Calculator/      # BMI + calorie estimator
│   ├── Gallery/         # Photo gallery + lightbox
│   ├── Testimonials/    # Member reviews
│   ├── FAQ/             # Accordion
│   ├── EnquirySection/  # Lead capture form
│   ├── Location/        # Map embed
│   ├── FinalCTA/        # Closing conversion
│   └── ...              # + 15 more utility components
├── data/
│   └── gym.ts           # 🔑 Central data file — edit here
├── config/
│   └── theme.ts         # Brand tokens / colors
└── utils/
    └── whatsapp.ts      # WhatsApp deep-link helper
```

---

## ✏️ Customising for a Real Gym

All demo content lives in **[`src/data/gym.ts`](./src/data/gym.ts)**. Change:

- `gym.name`, `gym.tagline` — Brand name
- `gym.contact` — Phone, email, WhatsApp, address
- `gym.programs` — Training programs
- `gym.trainers` — Trainer profiles + certifications
- `gym.memberships` — Pricing plans
- `gym.testimonials` — Member reviews
- `gym.schedule` — Weekly class timetable

> Set `DEMO_MODE = false` in `gym.ts` to remove the demo banner.

---

## 🔒 Security Headers

Pre-configured in `vercel.json`:
- `X-Frame-Options: DENY`
- `X-Content-Type-Options: nosniff`
- `X-XSS-Protection: 1; mode=block`
- `Referrer-Policy: strict-origin-when-cross-origin`
- `Permissions-Policy`: camera, mic, geolocation blocked
- Asset caching: **1 year immutable** for all `/assets/*`

---

## 📄 License

Built by **KSJ Technologies** — Sales demo. Not for redistribution.
