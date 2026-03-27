# Next.js Starter Template

A clean, production-ready Next.js 14 starter with the most common setup already done.

## What's Included

- ✅ Next.js 14 (App Router)
- ✅ TypeScript
- ✅ Tailwind CSS
- ✅ ESLint + Prettier
- ✅ Folder structure for scalable apps
- ✅ Environment variable setup
- ✅ Basic layout with header and footer

## Prompt to Generate This

Use this prompt with Claude or Cursor to scaffold this template:

```
Create a Next.js 14 starter project with:
- TypeScript enabled
- Tailwind CSS configured
- App Router structure
- A clean folder structure: app/, components/, lib/, types/, hooks/
- A basic layout.tsx with a Header and Footer component
- An index page that looks professional
- .env.local.example with common variable placeholders
- ESLint and Prettier config files
- A useful README.md

Make the UI clean and modern using Tailwind. 
No external UI libraries — just Tailwind utility classes.
```

## Folder Structure

```
my-app/
├── app/
│   ├── layout.tsx        # Root layout
│   ├── page.tsx          # Home page
│   ├── globals.css       # Global styles
│   └── (routes)/         # Your pages go here
├── components/
│   ├── ui/               # Reusable UI components
│   └── layout/           # Header, Footer, Nav
├── lib/
│   └── utils.ts          # Utility functions
├── hooks/                # Custom React hooks
├── types/                # TypeScript type definitions
├── public/               # Static assets
├── .env.local.example    # Environment variable template
└── next.config.js        # Next.js configuration
```

## Getting Started

```bash
npx create-next-app@latest my-app --typescript --tailwind --eslint --app
cd my-app
npm run dev
```
