# 🔌 API Integration Prompts

Connect your app to any external service quickly and safely.

---

## 1. API Integration Scaffold

**Best for:** Connecting to any third-party API  
**Works with:** Claude, ChatGPT, Cursor

```
Help me integrate [API NAME] into my [Next.js / Node.js] app.

What I want to do: [e.g. send emails, process payments, get weather data]
API docs URL (if you know it): [URL or "I'll paste the relevant docs below"]
[paste any relevant API docs]

Please:
1. Install instructions (what package to install)
2. Environment variables needed (.env keys)
3. A reusable service file that wraps the API
4. An example API route that uses it
5. Error handling for common failures (rate limit, auth error, network error)

Make it production-safe — no API keys hardcoded.
```

---

## 2. Webhook Handler

**Best for:** Stripe, GitHub, Clerk, or any webhook  
**Works with:** Claude, ChatGPT

```
Create a webhook handler for [SERVICE NAME] in Next.js.

Webhook events I need to handle:
- [event 1, e.g. payment.succeeded]
- [event 2, e.g. user.created]
- [event 3, e.g. subscription.cancelled]

For each event I need to: [describe what should happen]

Requirements:
- Verify webhook signature for security
- Return 200 fast, process async if needed
- Log events for debugging
- Handle duplicate events safely (idempotency)

Use Next.js App Router API route format.
```

---

## 3. Authentication Setup

**Best for:** Adding auth to any app  
**Works with:** Claude, ChatGPT, Cursor

```
Set up authentication in my Next.js app using [Clerk / NextAuth / Supabase Auth].

I need:
- Sign up / Sign in / Sign out flows
- Protected routes (redirect to login if not authenticated)
- User object available in: [server components / client components / API routes / all]
- [OAuth providers if needed: Google, GitHub, etc.]

Please give me:
1. Installation and environment setup
2. Provider/middleware configuration
3. Example protected page
4. Example of getting the user in an API route
5. Any common gotchas for this auth library
```

---

## 4. Data Fetching Layer

**Best for:** Organizing how your app fetches and caches data  
**Works with:** Claude, ChatGPT

```
Help me set up a clean data fetching layer for my Next.js app.

I need to fetch data from: [REST API / Supabase / your own API / etc.]
Data I need: [describe the main data types]
Caching strategy: [real-time / ISR / static / no cache]

Please create:
1. A reusable fetch utility with error handling
2. TypeScript types for API responses
3. Example server component that fetches data
4. Example client component with loading/error states
5. How to handle auth headers in requests

Use Next.js 14 App Router patterns.
```
