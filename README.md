# 🌿 AI NutriScan

> **Eat Smarter. Live Better. Scan Once.**

AI NutriScan is an AI-powered nutrition intelligence app that instantly analyses any meal from a photo — delivering a complete breakdown of calories, macros, and micronutrients in under 3 seconds. No manual logging. No guesswork. Just point, scan, and know exactly what you're eating.

[![Featured on Orynth](https://orynth.dev/api/badge/nutriscan-ai?theme=light&style=default)](https://orynth.dev/projects/nutriscan-ai)
[![Follow on X](https://img.shields.io/badge/Follow-%40nutriscandotfun-black?style=flat&logo=x)](https://x.com/nutriscandotfun)
[![GitHub Stars](https://img.shields.io/github/stars/ainutriscan/ainutriscan?style=flat&color=22c55e)](https://github.com/ainutriscan/ainutriscan)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📸 Screenshots

| Hero | Phone Mockup | Roadmap |
|------|-------------|---------|
| ![Cover](nutriscan_cover.jpg) | Scan · Analyse · Track | March → April 2026 |

---

## ✨ Features

- **📷 Instant Photo Scanning** — Identify any meal from a single photo in under 3 seconds
- **📊 Full Macro Dashboard** — Calories, protein, carbs, fat, fibre, vitamins & minerals
- **🤖 AI Nutrition Insights** — Personalised recommendations that learn your eating habits
- **🌾 Farm-to-Table Tracing** — Full ingredient traceability from field to plate
- **🍽️ Restaurant Menu Scanner** — Real-time nutrition info at partner restaurants & warungs
- **🎓 Campus Programme** — University partnerships for canteens & nutrition research

---

## 🗺️ Roadmap 2026

| Date | Milestone | Status |
|------|-----------|--------|
| **March 2026** | 🚀 Official Launch — Orynth | ✅ Live |
| **April (Early)** | 🎓 Campus Partnership Programme | 🔜 Coming Soon |
| **April (Mid)** | 🌾 Farmer & Supply Chain Integration | 🔜 Coming Soon |
| **April (Mid)** | 🍽️ Restaurant & Warung Network | 🔜 Coming Soon |
| **April (Late)** | 💱 Exchange Listing | 🔥 High Impact |
| **Q3 2026** | 🌏 National Expansion (10 cities) | 📋 Planned |

---

## 🚀 Getting Started

### Prerequisites

- Node.js v18+
- npm or yarn
- iOS 15+ / Android 10+

### Installation

```bash
# Clone the repository
git clone https://github.com/ainutriscan/ainutriscan.git
cd ainutriscan

# Install dependencies
npm install

# Copy environment variables
cp .env.example .env

# Start development server
npm run dev
```

### Environment Variables

```env
NEXT_PUBLIC_API_URL=https://api.nutriscan.ai
NEXT_PUBLIC_APP_ENV=development
AI_MODEL_ENDPOINT=your_model_endpoint
DATABASE_URL=your_database_url
NEXTAUTH_SECRET=your_secret_key
NEXTAUTH_URL=http://localhost:3000
```

---

## 🏗️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | Next.js 14, TypeScript, Tailwind CSS |
| Mobile | React Native (iOS & Android) |
| AI / ML | PyTorch, Custom Vision Transformer |
| Backend | Node.js, FastAPI (Python) |
| Database | PostgreSQL, Redis |
| Storage | AWS S3 |
| Auth | NextAuth.js |
| Deployment | Vercel (Frontend), AWS (Backend) |

---

## 📁 Project Structure

```
ainutriscan/
├── apps/
│   ├── web/                 # Next.js landing page & dashboard
│   └── mobile/              # React Native app (iOS + Android)
├── packages/
│   ├── ai-core/             # Vision AI model & inference
│   ├── nutrition-db/        # Food & nutrition database
│   └── ui/                  # Shared component library
├── services/
│   ├── api/                 # REST API (FastAPI)
│   ├── auth/                # Authentication service
│   └── tracing/             # Farm-to-table traceability
├── docs/                    # Documentation
├── .env.example
├── package.json
└── README.md
```

---

## 🤝 Team

| Name | Role | Location |
|------|------|----------|
| **Nana Beauchamp-Tremblay** | CEO & Co-Founder | Vancouver, Canada 🇨🇦 |
| **Liam Okonkwo-Pearce** | CTO & Co-Founder | Toronto, Canada 🇨🇦 |
| **Zoé Larivière-Bouchard** | Head of Design | Montréal, Canada 🇨🇦 |

Follow us on X: [@nutriscandotfun](https://x.com/nutriscandotfun)

---

## 💰 Pricing

| Plan | Price | Scans | Features |
|------|-------|-------|----------|
| **Starter** | Free | 5/day | Basic macros, 7-day history |
| **Pro** | Rp 49K/month | Unlimited | Full nutrients, AI insights, tracing, PDF reports |

---

## 🔌 API Reference

### Scan a Food Image

```http
POST /api/v1/scan
Authorization: Bearer {token}
Content-Type: multipart/form-data
```

**Request:**
```json
{
  "image": "<base64_or_file>",
  "serving_size": "medium"
}
```

**Response:**
```json
{
  "food_name": "Nasi Goreng Kampung",
  "confidence": 0.97,
  "serving_size_g": 280,
  "nutrition": {
    "calories": 482,
    "protein_g": 18.4,
    "carbs_g": 64.2,
    "fat_g": 16.8,
    "fiber_g": 3.1,
    "sodium_mg": 820
  },
  "ingredients": ["rice", "egg", "garlic", "shallot", "kecap manis"],
  "origin_trace": {
    "farm": "Pak Hendra Organics",
    "location": "Malang, East Java",
    "freshness_score": 94
  }
}
```

### Get Meal History

```http
GET /api/v1/history?date=2026-03-20&limit=10
Authorization: Bearer {token}
```

---

## 🌍 Localisation

AI NutriScan natively supports:
- 🇮🇩 Indonesian (Bahasa Indonesia)
- 🇬🇧 English
- 🇸🇦 Arabic *(coming Q3 2026)*
- 🇲🇾 Malay *(coming Q3 2026)*

---

## 🛡️ Privacy & Security

- All images are processed server-side and **never stored permanently** without consent
- Nutrition data is encrypted at rest (AES-256) and in transit (TLS 1.3)
- GDPR & UU PDP (Indonesian Personal Data Protection Law) compliant
- Users can export or permanently delete all data at any time

---

## 🤝 Contributing

We welcome contributions! Please read our [Contributing Guide](CONTRIBUTING.md) before submitting a PR.

```bash
# Fork the repo, then:
git checkout -b feature/your-feature-name
git commit -m "feat: add your feature"
git push origin feature/your-feature-name
# Open a Pull Request on GitHub
```

---

## 📬 Contact & Community

| Channel | Link |
|---------|------|
| 𝕏 Twitter / X | [@nutriscandotfun](https://x.com/nutriscandotfun) |
| GitHub | [ainutriscan/ainutriscan](https://github.com/ainutriscan/ainutriscan) |
| Orynth | [orynth.dev/projects/nutriscan-ai](https://orynth.dev/projects/nutriscan-ai) |
| Email | hello@nutriscan.ai |

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

<div align="center">
  <strong>Built with ❤️ by the AI NutriScan team · Launching from Orynth 🌿</strong><br/>
  <a href="https://orynth.dev/projects/nutriscan-ai">
    <img src="https://orynth.dev/api/badge/nutriscan-ai?theme=light&style=default" alt="Featured on Orynth" width="200" height="56"/>
  </a>
</div>
