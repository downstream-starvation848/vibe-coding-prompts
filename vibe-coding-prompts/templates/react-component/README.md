# React Component Template

A standard template for creating consistent, well-typed React components.

## The Template

```tsx
// components/ui/ComponentName.tsx

import { ReactNode } from 'react'

// 1. Define your props interface
interface ComponentNameProps {
  // Required props
  title: string
  
  // Optional props (use ?)
  description?: string
  className?: string
  children?: ReactNode
  
  // Event handlers
  onClick?: () => void
}

// 2. Build the component
export function ComponentName({ 
  title, 
  description, 
  className = '',
  children,
  onClick 
}: ComponentNameProps) {
  
  return (
    <div className={`/* base styles */ ${className}`}>
      <h2>{title}</h2>
      {description && <p>{description}</p>}
      {children}
      {onClick && (
        <button onClick={onClick}>
          Action
        </button>
      )}
    </div>
  )
}

// 3. Default export (optional — use named exports for tree-shaking)
export default ComponentName
```

## Prompt to Generate a Component

```
Create a [COMPONENT NAME] React component following this structure:

Props needed:
- [prop name]: [type] — [description]
- [prop name]: [type] — [description]

The component should:
- [describe visual appearance]
- [describe behavior]
- Accept a className prop for customization
- Be fully typed with TypeScript

Use Tailwind CSS for styling. Export as a named export.
```

## Component Checklist

Before shipping a component, check:
- [ ] All props have TypeScript types
- [ ] Optional props have default values
- [ ] Component accepts `className` for customization
- [ ] Loading state handled (if async data)
- [ ] Empty state handled (if showing a list)
- [ ] Error state handled (if can fail)
- [ ] Accessible: has proper aria labels if needed
- [ ] Responsive: works on mobile and desktop
