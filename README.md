# ReBap (Resume Build App)

> Recreate and build professional resumes with Gemini AI.

![Version](https://img.shields.io/badge/version-0.1.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![React](https://img.shields.io/badge/React-18-61dafb)

---

## ✨ Features

- 📄 Upload an existing resume (PDF or image)
- 🤖 AI-powered resume analysis and reconstruction with Gemini
- ✏️ Visual section-by-section editor
- 🎨 Customize colors, fonts, and layout
- 📥 PDF export
- 🔐 Secure authentication with Supabase
- 📱 Progressive Web App (installable)

---

## 🛠️ Tech Stack

| Role                      | Technology                   |
| ------------------------- | ---------------------------- |
| Frontend                  | React 18 + Vite + TypeScript |
| Styling                   | Tailwind CSS v3              |
| Animations                | Framer Motion                |
| State Management          | Zustand                      |
| Routing                   | React Router v6              |
| Authentication & Database | Supabase                     |
| AI                        | Gemini 2.0 Flash             |
| PDF Export                | @react-pdf/renderer          |
| PWA                       | vite-plugin-pwa              |

---

## 🚀 Installation

### Prerequisites

- Node.js 18+
- A free Supabase account
- A free Gemini API key

### Setup

```bash
# 1. Clone the repository
git clone https://github.com/brondonnono/rebap.git
cd rebap

# 2. Install dependencies
npm install

# 3. Configure environment variables
cp .env.example .env

# Fill in:
# VITE_SUPABASE_URL
# VITE_SUPABASE_ANON_KEY

# 4. Start the development server
npm run dev
```

---

## 📁 Project Structure

```text
src/
├── components/     # Reusable components
│   ├── ui/         # Buttons, inputs, cards...
│   ├── layout/     # Navbar, sidebar...
│   └── cv/         # Resume-specific components
├── pages/          # One page = one route
├── store/          # Global state management (Zustand)
├── hooks/          # Reusable business logic
├── lib/            # External clients (Supabase, Gemini)
└── types/          # Shared TypeScript types
```

## 🔐 Security

- The Gemini API key is stored **in memory only** (never in localStorage)
- Row Level Security (RLS) is enabled on all Supabase tables
- No secrets are exposed on the client side

---

## 📖 Documentation

- [Contribution Guide](./CONTRIBUTING.md)
- [Detailed Architecture](./docs/ARCHITECTURE.md)

---

## 📄 License

MIT — see [LICENSE](./LICENSE)
