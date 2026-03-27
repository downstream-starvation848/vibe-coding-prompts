# 🗄️ Database Prompts

Design schemas, write queries, and manage your data layer.

---

## 1. Schema Designer

**Best for:** Planning your database before you build  
**Works with:** Claude, ChatGPT

```
Design a database schema for my app: [APP NAME]

Core features:
- [feature 1]
- [feature 2]
- [feature 3]

Database: [PostgreSQL / MySQL / MongoDB / Supabase]

Please provide:
1. All tables/collections with fields and data types
2. Primary keys and foreign keys
3. Indexes for performance (explain why each is needed)
4. Any junction tables for many-to-many relationships
5. Fields to add for soft deletes, timestamps, audit trails

Output as SQL CREATE TABLE statements (or MongoDB schema format).
Flag any design decisions I should think about before committing.
```

---

## 2. Query Optimizer

**Best for:** Slow database queries  
**Works with:** Claude, ChatGPT

```
Optimize this database query:

[paste query]

Context:
- Database: [PostgreSQL / MySQL / SQLite]
- Table sizes: [approximate row counts]
- Current performance: [e.g. "takes 3 seconds"]
- Indexes that exist: [list them]

Please:
1. Explain why the query is slow
2. Rewrite it to be faster
3. Suggest any indexes to add
4. Show the EXPLAIN ANALYZE output I should look for to confirm improvement
```

---

## 3. Supabase Setup Guide

**Best for:** New Supabase projects  
**Works with:** Claude, ChatGPT

```
Help me set up Supabase for my Next.js app.

I need:
- Tables: [list your main data types]
- Auth: [email/password / OAuth / magic link]
- Row Level Security policies for: [describe who can see/edit what]
- Real-time subscriptions: [yes/no — for what data]

Please provide:
1. SQL to create all tables
2. RLS policies for each table
3. Next.js environment setup
4. Supabase client initialization (server + client)
5. Example of CRUD operations for my main data type

Make the RLS policies secure by default.
```
