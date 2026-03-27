# ♻️ Refactoring Prompts

Clean up messy code and make it maintainable.

---

## 1. Clean Code Refactor

**Best for:** Any messy, hard-to-read code  
**Works with:** Claude, ChatGPT, Cursor

```
Refactor this code to be cleaner and more maintainable:

[paste code]

Goals:
- Better variable/function names
- Break large functions into smaller ones
- Remove duplication (DRY principle)
- Add TypeScript types if missing
- Add JSDoc comments for complex logic

Keep the exact same functionality — don't change behavior, only code quality.
Show me a before/after and explain each change.
```

---

## 2. Component Splitter

**Best for:** Giant React components that do too much  
**Works with:** Claude, ChatGPT, Cursor

```
This React component is too large. Please split it into smaller components:

[paste component code]

Rules:
- Each new component should have one clear responsibility
- Keep props minimal and well-typed
- Use proper component naming conventions
- Decide what state should live where
- Keep the folder structure clean

Show me the final file structure and all new component files.
```

---

## 3. JavaScript to TypeScript Migration

**Best for:** Adding types to existing JS code  
**Works with:** Claude, ChatGPT, Cursor

```
Convert this JavaScript to TypeScript:

[paste JS code]

Requirements:
- Add proper types for all variables, parameters, and return values
- Create interfaces/types for data objects
- Handle null/undefined cases properly
- Use generics where appropriate
- Don't use `any` unless truly necessary — explain when you do

Show me the typed version with comments explaining key type decisions.
```

---

## 4. API Route Cleaner

**Best for:** Messy Next.js API routes or Express endpoints  
**Works with:** Claude, ChatGPT

```
Refactor this API route to be production-ready:

[paste API route code]

Improve:
1. Input validation (add Zod or manual checks)
2. Error handling (proper HTTP status codes and messages)
3. Response format consistency
4. Remove any logic that doesn't belong in the route
5. Add TypeScript types
6. Security: check for auth, rate limiting needs

Give me the cleaned-up version with explanations.
```
