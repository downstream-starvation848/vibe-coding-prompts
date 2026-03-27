# 🔍 Code Review Prompts

Use these before shipping. Catch problems before your users do.

---

## 1. Full Code Review

**Best for:** Any file or feature before merging  
**Works with:** Claude, ChatGPT, Cursor

```
Please do a thorough code review of the following code:

[paste code]

Review it for:
1. **Bugs** — logic errors, edge cases, off-by-one errors
2. **Security** — XSS, SQL injection, exposed secrets, unsafe inputs
3. **Performance** — unnecessary re-renders, expensive operations, N+1 queries
4. **Readability** — naming, complexity, missing comments
5. **Best practices** — for [React / Next.js / Node / etc.]

Format your response as:
- 🔴 Critical (must fix before shipping)
- 🟡 Warning (should fix soon)
- 🟢 Suggestion (nice to have)

Then give me the improved version of the code.
```

---

## 2. Security Audit

**Best for:** Authentication, forms, API routes, user data  
**Works with:** Claude, ChatGPT

```
Audit this code for security vulnerabilities:

[paste code]

This code handles: [e.g. user authentication / payment data / file uploads / API keys]

Check specifically for:
- Exposed sensitive data (API keys, passwords, PII)
- Missing input validation/sanitization
- Improper authentication checks
- CORS issues
- Rate limiting gaps
- Insecure direct object references

List every vulnerability found, severity level, and the exact fix.
```

---

## 3. Performance Review

**Best for:** Slow components, expensive pages  
**Works with:** Claude, ChatGPT, Cursor

```
Review this code for performance issues:

[paste code]

Context:
- This is a: [React component / API route / database query / etc.]
- It runs: [on every render / once on load / per user action]
- Current problem: [it feels slow / it re-renders too much / etc.]

Find all performance issues and rewrite the code with fixes applied.
Explain each optimization you made and why it helps.
```

---

## 4. Pre-Launch Checklist Generator

**Best for:** Before going live  
**Works with:** Claude, ChatGPT

```
I'm about to launch [APP NAME]. It's built with [TECH STACK].

Generate a pre-launch checklist covering:
1. Security (auth, env vars, HTTPS, headers)
2. Performance (images, caching, bundle size)
3. SEO (meta tags, og tags, sitemap, robots.txt)
4. Accessibility (contrast, keyboard nav, screen readers)
5. Error handling (404, 500, form errors)
6. Analytics & monitoring setup
7. Backup and recovery plan

Mark each item as [required / recommended / optional].
```
