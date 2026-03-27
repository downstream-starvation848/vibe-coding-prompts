# 🚀 Deployment Prompts

Ship your app to the world, safely and confidently.

---

## 1. Vercel Deployment Guide

**Best for:** Deploying Next.js apps  
**Works with:** Claude, ChatGPT

```
Help me deploy my Next.js app to Vercel.

My app uses:
- Database: [Supabase / PlanetScale / Neon / none]
- Auth: [Clerk / NextAuth / Supabase Auth / none]
- Environment variables: [list the keys, not the values]
- External APIs: [list services]

Please give me:
1. Pre-deployment checklist
2. Which environment variables to add in Vercel dashboard
3. Any build configuration needed (next.config.js changes)
4. How to set up preview deployments for branches
5. Common deployment errors for this stack and how to fix them

I want zero-downtime deployments.
```

---

## 2. Environment Variables Audit

**Best for:** Before making a repo public or deploying  
**Works with:** Claude, ChatGPT

```
Audit my environment variable usage for security:

My .env.local file has these keys (NOT values):
[list your env var key names]

My tech stack: [Next.js / Node / etc.]

Please:
1. Flag any that should NEVER be exposed to the client (no NEXT_PUBLIC_ prefix)
2. Identify any that are safe to be public
3. Check if my usage pattern is secure
4. Generate a proper .env.example file
5. Tell me what to add to .gitignore

Make sure I don't accidentally leak secrets.
```

---

## 3. CI/CD Pipeline Setup

**Best for:** Automating tests and deployments  
**Works with:** Claude, ChatGPT

```
Set up a CI/CD pipeline for my [Next.js / Node.js] project using GitHub Actions.

I want it to:
- Run on: [every push / only on PRs / only on main branch]
- Steps: [lint, type check, tests, build, deploy]
- Deploy to: [Vercel / Railway / Fly.io / custom server]
- Notify me on: [failure only / always]

Please create the GitHub Actions YAML file and explain each step.
Include how to securely store secrets in GitHub.
```
