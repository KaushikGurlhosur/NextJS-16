## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Concepts:

## 🚀 Next.js 16 Routing Enhancements

### Layout Deduplication

In Next.js 16, shared layouts are no longer re-rendered when navigating between nested routes.  
Only the leaf page updates, resulting in faster transitions and smoother UX.

**Example:**
Navigating from `/dashboard/users` → `/dashboard/analytics` keeps the `dashboard/layout.tsx` mounted and persistent.

### Incremental Prefetching

Next.js 16 introduces intelligent prefetching:

- Routes are prefetched **incrementally** as links enter the viewport.
- Metadata loads first, followed by route chunks on hover or near scroll.
- Network-aware and bandwidth-efficient.
