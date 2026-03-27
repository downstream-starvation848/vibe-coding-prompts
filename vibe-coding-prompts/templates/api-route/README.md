# API Route Template

A production-ready template for Next.js App Router API routes.

## The Template

```typescript
// app/api/[route-name]/route.ts

import { NextRequest, NextResponse } from 'next/server'

// GET handler
export async function GET(request: NextRequest) {
  try {
    // 1. Parse query params
    const { searchParams } = new URL(request.url)
    const id = searchParams.get('id')

    // 2. Validate input
    if (!id) {
      return NextResponse.json(
        { error: 'Missing required parameter: id' },
        { status: 400 }
      )
    }

    // 3. Do your logic here
    const data = await fetchSomeData(id)

    // 4. Return success response
    return NextResponse.json({ data }, { status: 200 })

  } catch (error) {
    console.error('[GET /api/route-name]', error)
    return NextResponse.json(
      { error: 'Internal server error' },
      { status: 500 }
    )
  }
}

// POST handler
export async function POST(request: NextRequest) {
  try {
    // 1. Parse request body
    const body = await request.json()
    const { name, email } = body

    // 2. Validate input
    if (!name || !email) {
      return NextResponse.json(
        { error: 'Missing required fields: name, email' },
        { status: 400 }
      )
    }

    // 3. Do your logic here
    const result = await createSomething({ name, email })

    // 4. Return success response
    return NextResponse.json({ result }, { status: 201 })

  } catch (error) {
    console.error('[POST /api/route-name]', error)
    return NextResponse.json(
      { error: 'Internal server error' },
      { status: 500 }
    )
  }
}

// Placeholder — replace with real implementation
async function fetchSomeData(id: string) {
  return { id, message: 'Replace this with real data fetching' }
}

async function createSomething(data: { name: string; email: string }) {
  return { ...data, id: crypto.randomUUID() }
}
```

## Prompt to Generate an API Route

```
Create a Next.js App Router API route for: [DESCRIBE WHAT IT DOES]

Endpoint: [e.g. POST /api/users]
Input: [describe the request body or query params]
Output: [describe what it should return]
Auth required: [yes/no]

Include:
- Input validation
- Proper error handling with correct HTTP status codes
- TypeScript types
- Comments explaining the logic

Use the Next.js 14 App Router format (not Pages Router).
```

## HTTP Status Code Reference

| Code | Use When |
|------|----------|
| 200 | Successful GET / update |
| 201 | Successfully created a resource |
| 400 | Bad request (missing/invalid input) |
| 401 | Not authenticated |
| 403 | Authenticated but not authorized |
| 404 | Resource not found |
| 409 | Conflict (e.g. duplicate email) |
| 500 | Unexpected server error |
