# 🐛 Debugging Prompts

Use these when something is broken and you can't figure out why.

---

## 1. The Bug Terminator

**Best for:** Any bug, any language  
**Works with:** Claude, ChatGPT, Cursor

```
I have a bug and I can't figure it out. Here's everything:

**What I expected:** [describe expected behavior]
**What actually happens:** [describe actual behavior]
**Error message (if any):** [paste full error]
**Relevant code:** 
[paste code here]

**What I've already tried:** [list your attempts]
**Stack:** [e.g. Next.js 14, Node 20, Supabase]

Please:
1. Identify the root cause
2. Explain WHY it's happening in simple terms
3. Give me the exact fix with code
4. Tell me how to avoid this class of bug in the future
```

---

## 2. Console Error Decoder

**Best for:** Cryptic error messages  
**Works with:** Claude, ChatGPT

```
I'm getting this error and I don't understand it:

[PASTE FULL ERROR MESSAGE AND STACK TRACE]

Context:
- What I was doing when it happened: [DESCRIBE]
- Framework/language: [e.g. Next.js, TypeScript]
- Relevant file: [paste relevant code]

Please:
1. Explain what this error means in plain English
2. Tell me exactly where in my code the problem is
3. Give me the fix
4. Explain if this could cause other problems
```

---

## 3. Why Is My UI Broken?

**Best for:** Layout and styling issues  
**Works with:** Claude, ChatGPT, Cursor

```
My UI looks wrong. Here's the situation:

**Expected:** [describe how it should look]
**Actual:** [describe how it looks now]
**Component code:**
[paste JSX/HTML]

**CSS/Tailwind classes:**
[paste styles]

**Browser:** [Chrome/Firefox/Safari]
**Screen size issue?** [yes/no]

Find the styling bug and fix it. Explain what was wrong.
```

---

## 4. Async/Promise Debugger

**Best for:** Async bugs, race conditions, loading issues  
**Works with:** Claude, ChatGPT

```
I have an async bug. Here's what's happening:

**The problem:** [data not loading / wrong order / undefined errors / etc.]
**My code:**
[paste async code]

**Error (if any):** [paste error]

Please:
1. Identify the async issue (race condition, missing await, etc.)
2. Explain the timing problem in simple terms
3. Rewrite the code correctly
4. Add proper error handling if missing
```

---

## 5. Performance Debugger

**Best for:** Slow pages, laggy UI, memory leaks  
**Works with:** Claude, ChatGPT

```
My app is [slow / laggy / crashing after a while].

**Where I notice it:** [page name / action that causes it]
**Component/code involved:**
[paste code]

**What I've already checked:** [list]

Please:
1. Identify likely performance issues in my code
2. Rank them by impact (high/medium/low)
3. Rewrite the problematic sections with fixes
4. Suggest what to measure with DevTools to confirm
```
