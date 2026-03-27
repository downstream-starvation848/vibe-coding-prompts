# 🎨 UI Generation Prompts

Use these to build beautiful interfaces fast with AI tools.

---

## 1. Component Generator (Tailwind + React)

**Best for:** Any UI component  
**Works with:** Claude, v0, Cursor

```
Create a [COMPONENT NAME] component for my React/Next.js app.

Requirements:
- Style: [modern / minimal / glassmorphism / dark / brutalist / soft]
- Must include: [list features e.g. hover states, icons, loading state]
- Props it should accept: [list props with types]
- Responsive: [yes - mobile first / desktop only]
- Animations: [none / subtle / bold]
- Color scheme: [your colors or "use a nice default"]

Use Tailwind CSS only (no custom CSS).
Make it accessible (proper aria labels, keyboard nav).
Export it as a named export.
```

---

## 2. Full Page Layout Builder

**Best for:** Landing pages, dashboards, marketing pages  
**Works with:** Claude, v0, ChatGPT

```
Build a complete [PAGE TYPE] page for [APP/PRODUCT NAME].

Page purpose: [what this page should achieve]
Target audience: [who will see this]

Sections to include:
- [section 1, e.g. Hero with CTA]
- [section 2, e.g. Features grid]
- [section 3, e.g. Testimonials]
- [section 4, e.g. Pricing]
- [section 5, e.g. Footer]

Style: [describe the vibe — e.g. "like Linear.app, dark, minimal"]
Tech: Next.js 14 + Tailwind CSS
Include: Responsive design, smooth scroll, subtle animations

Make it look like it was designed by a professional.
```

---

## 3. Dashboard UI Generator

**Best for:** Admin panels, analytics, internal tools  
**Works with:** Claude, v0, Cursor

```
Create a dashboard UI for [APP NAME].

Data to display:
- [metric 1, e.g. Total Users: number]
- [metric 2, e.g. Revenue: chart]
- [metric 3, e.g. Recent activity: table]

Layout: [sidebar nav / top nav / both]
Theme: [dark / light / system]
Charts needed: [line chart / bar chart / donut / none]

Use: React + Tailwind CSS
Include: Responsive sidebar collapse on mobile, loading skeletons

Make the stats cards visually distinct and easy to scan.
```

---

## 4. Form Builder

**Best for:** Sign up, contact, checkout, onboarding forms  
**Works with:** Claude, ChatGPT, Cursor

```
Build a [FORM TYPE] form component.

Fields needed:
- [field 1: type, label, validation]
- [field 2: type, label, validation]
- [field 3: type, label, validation]

Requirements:
- Validation: [real-time / on submit]
- Error messages: [inline / toast]
- Loading state on submit: yes/no
- Success state: [redirect / success message]
- Library: [React Hook Form / plain React state]

Style with Tailwind. Make errors clear and UX smooth.
```

---

## 5. Navigation Component

**Best for:** Headers, sidebars, mobile menus  
**Works with:** Claude, v0

```
Create a navigation component for my app.

Type: [top navbar / sidebar / bottom mobile nav / all three]
Links: [Home, About, Pricing, Dashboard, Login, etc.]
Features needed:
- Mobile hamburger menu: yes/no
- Active link highlighting: yes/no
- User avatar/dropdown: yes/no
- Search bar: yes/no
- Dark mode toggle: yes/no

Logo: [text only / image placeholder]
Style: [sticky / static / transparent on hero]

Use Next.js Link component + Tailwind CSS.
```

---

## 6. Loading & Empty States

**Best for:** Better UX while data loads or is missing  
**Works with:** Claude, ChatGPT

```
Create loading and empty state components for [COMPONENT NAME].

Loading state:
- Type: [skeleton / spinner / pulse animation]
- Match the layout of: [describe the real component]

Empty state:
- Message: [e.g. "No projects yet"]
- CTA button: [e.g. "Create your first project"]
- Include an illustration or icon: yes/no

Make them feel intentional, not like afterthoughts.
Use Tailwind CSS.
```
