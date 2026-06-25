<div align="center">

# ⚡ CONJURE

**AI-Native Form & Survey Platform**

Type one sentence. Get a production-ready form in under 10 seconds.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-FF6B35?style=for-the-badge&logo=vercel&logoColor=white)](https://app-ck0zz2f81wqp.appmedo.com)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=white)](https://react.dev)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.9-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://typescriptlang.org)
[![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)](https://supabase.com)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.4-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com)

</div>

---

## 🚀 Live Demo

**[https://app-ck0zz2f81wqp.appmedo.com](https://app-ck0zz2f81wqp.appmedo.com)**

No installation required. Open the link, type your form idea, and watch AI generate it instantly.

---

## ✨ What is Conjure?

Conjure is an AI-native form platform that eliminates the drag-and-drop grind. Instead of building forms field by field, you **describe what you need in plain English** and Gemini 2.5 Flash reasons about your intent, selects optimal field types, orders questions logically, wires conditional logic, and produces a production-ready form schema — all in under 10 seconds.

### The Problem

Traditional form builders force users into a manual, repetitive workflow:
- Blank canvas → pick fields one by one
- Write every question manually
- Wire conditional logic by hand
- No AI insights on collected data
- Anyone with a link can see responses

### Our Solution

- **One-sentence generation** → full form instantly
- **AI writes questions**, picks types, orders logically
- **Conditional logic auto-wired** from your description
- **Live real-time response table** with zero refresh
- **AI summary** of trends and outliers
- **Row-Level Security** — only form owners see responses

---

## 🎯 Key Features

| Feature | Description |
|---------|-------------|
| **⚡ AI Form Generation** | Type a description. Gemini 2.5 Flash generates the complete form schema with fields, validation, and conditional logic. |
| **🎨 Advanced Visual Customization** | Background images, overlay opacity, CSS patterns (dots/stripes/grid/noise), custom logo, button styles (solid/outline/ghost), and field entrance animations. |
| **🖋️ Typography Engine** | Per-element font family & size controls for headings, body text, and labels with live preview. |
| **🌗 Light / Dark Mode** | Toggle between light and dark themes per form. Preview updates instantly in the Studio. |
| **🛡️ Auth & Ownership** | Email/password + Google OAuth. Forms tied to authenticated accounts. RLS enforces owner-only access. |
| **📊 Real-Time Responses** | Live Supabase Realtime subscriptions stream responses as they arrive. Search, filter, sort, CSV/Excel export. |
| **📈 Analytics Dashboard** | Visual charts (Recharts) showing response distribution, completion rates, and field-level statistics. |
| **🗂️ Template Gallery** | Pre-built form templates for common use cases. |
| **💬 AI Form Editor** | Chat-based editing — describe changes and the AI updates the form fields for you. |
| **🎭 Brutalism Design System** | Premium high-contrast theme with razor borders, offset shadows, and Space Grotesk + Anton typography. |
| **🧩 20+ Field Types** | Short text, long text, email, number, date, dropdown, multiple choice, checkbox, rating, NPS, slider, ranking, matrix, yes/no, statement, phone, address, file upload, signature, and more. |
| **📱 Responsive** | Fully responsive from mobile to desktop. |

---

## 🛠️ Technology Stack

| Layer | Technology |
|-------|------------|
| **Frontend** | React 18, TypeScript 5.9, Vite |
| **Styling** | Tailwind CSS 3.4, shadcn/ui, Brutalism Design System |
| **Backend** | Supabase (PostgreSQL, Auth, Realtime, Edge Functions, Storage) |
| **AI** | Gemini 2.5 Flash via Gateway (streaming SSE) |
| **Charts** | Recharts |
| **Animation** | Motion (Framer Motion) |
| **Icons** | Lucide React |
| **Notifications** | Sonner |
| **Routing** | React Router v7 |
| **HTTP Client** | Supabase Functions client, ky (SSE streaming) |
| **Linting** | Biome |

---

## 📁 Project Structure

```
conjure/
├── .env.example                  # Environment variables template
├── .gitignore                    # Git ignore rules
├── package.json                  # Dependencies & scripts
├── vite.config.ts               # Vite build configuration
├── tsconfig.json                # TypeScript configuration
├── tailwind.config.js           # Tailwind theme & design tokens
├── index.html                   # Entry HTML
├── postcss.config.js            # PostCSS configuration
├── components.json              # shadcn/ui configuration
├── biome.json                   # Biome linting configuration
├── public/                      # Static assets
├── src/
│   ├── main.tsx               # React entry point
│   ├── App.tsx                # Root app with providers
│   ├── routes.tsx             # Route definitions
│   ├── index.css              # Global styles + Brutalism design system
│   ├── pages/                 # Route-level pages
│   │   ├── LandingPage.tsx
│   │   ├── AuthPage.tsx
│   │   ├── DashboardPage.tsx
│   │   ├── GeneratePage.tsx
│   │   ├── StudioPage.tsx
│   │   ├── FormViewPage.tsx
│   │   ├── ResponsesPage.tsx
│   │   ├── AnalyticsPage.tsx
│   │   ├── TemplatesPage.tsx
│   │   └── NotFound.tsx
│   ├── components/            # Reusable UI components
│   │   ├── ui/                # shadcn/ui primitives
│   │   ├── ThemeCustomizer.tsx
│   │   ├── dropzone.tsx
│   │   └── common/            # RouteGuard, PageMeta, IntersectObserver
│   ├── contexts/
│   │   └── AuthContext.tsx    # Auth state (email + Google OAuth)
│   ├── hooks/                 # Custom React hooks
│   ├── lib/                   # Utilities (utils.ts, sse.ts)
│   ├── services/
│   │   └── api.ts             # Form CRUD, Supabase helpers
│   ├── db/
│   │   └── supabase.ts        # Supabase client singleton
│   └── types/                 # TypeScript definitions
└── supabase/
    ├── config.toml
    ├── migrations/
    │   ├── 00001_conjure_schema.sql
    │   └── 00002_auth_profiles_rls_realtime_themes.sql
    └── functions/
        ├── generate-form/
        ├── large-language-model/
        └── ai-insights/
```

---

## 🚦 Getting Started

### Prerequisites

- Node.js ≥ 20
- pnpm ≥ 9
- A Supabase project (free tier works)

### 1. Clone & Install

```bash
git clone <repository-url>
cd conjure
pnpm install
```

### 2. Configure Environment

```bash
cp .env.example .env
```

Edit `.env` and fill in your Supabase credentials:

```env
VITE_SUPABASE_URL=https://your-project.supabase.co
VITE_SUPABASE_ANON_KEY=your-anon-key
VITE_SENTRY_DSN=https://your-sentry-dsn.ingest.sentry.io/your-project-id
VITE_APP_ID=your-app-id
```

### 3. Set Up Database

Deploy the migrations to your Supabase project:

```bash
supabase migration up
```

Or run the SQL files in `supabase/migrations/` directly from the Supabase SQL Editor.

### 4. Deploy Edge Functions

```bash
supabase functions deploy generate-form
supabase functions deploy large-language-model
supabase functions deploy ai-insights
```

### 5. Start Development Server

```bash
pnpm exec vite
```

The app will be available at `http://localhost:5173`.

---

## 🏗️ Build & Deploy

```bash
# Lint check
pnpm run lint

# Production build
pnpm exec vite build
```

Deploy the `dist/` folder to Vercel, Netlify, Cloudflare Pages, or any static hosting.

---

## 🧠 AI Workflow

### Form Generation

1. User types a description in the Generate page
2. Frontend calls the `generate-form` Edge Function
3. Gemini 2.5 Flash returns a JSON schema with fields, types, and conditional logic
4. Schema is saved to `forms` table with `user_id = auth.uid()`
5. User is redirected to Studio for customization

### AI Chat Editing

1. User describes changes in the Studio AI Chat tab
2. Frontend calls `large-language-model` Edge Function via `supabase.functions.invoke`
3. Gemini returns the complete updated field array
4. Fields are parsed from JSON and applied to form state
5. Live preview updates instantly

---

## 🔒 Security

- **Row-Level Security (RLS)** on all tables — users only access their own data
- **Auth triggers** auto-create user profiles on signup
- **Edge Functions** validate ownership before mutations
- **No secrets in source** — all credentials via environment variables

---

## 🗺️ Roadmap

- [ ] Drag-and-drop field reordering
- [ ] Multi-language form support
- [ ] File upload fields with Supabase Storage
- [ ] Email notifications on new responses
- [ ] Public template marketplace
- [ ] Team/organization support
- [ ] Zapier / Make.com integrations
- [ ] Custom domain for published forms
- [ ] Advanced AI analytics with trend forecasting
- [ ] PDF export of individual responses

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

Please ensure `pnpm run lint` passes before submitting.

---

## 📄 License

This project is licensed under the MIT License.

---

## 🙏 Acknowledgements

- [shadcn/ui](https://ui.shadcn.com) — Beautiful, accessible UI primitives
- [Supabase](https://supabase.com) — Open-source Firebase alternative
- [Gemini](https://deepmind.google/technologies/gemini/) — Google's multimodal AI model
- [Tailwind CSS](https://tailwindcss.com) — Utility-first CSS framework
- [Framer Motion](https://motion.dev) — Production-ready animations
- [Lucide](https://lucide.dev) — Beautiful open-source icons

---

<div align="center">

Built with ⚡ by the Conjure team · **[Live Demo](https://app-ck0zz2f81wqp.appmedo.com)**

</div>
