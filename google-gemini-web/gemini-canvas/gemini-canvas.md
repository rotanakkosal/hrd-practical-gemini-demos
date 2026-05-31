# Canvas Use Cases for Full-Stack Students

A prompt library for learning and practicing full-stack development with Canvas.

---

## Next.js Concept Visualizers

**Server vs Client Components:**

```text
Build me an interactive Next.js component tree where I can toggle each node between Server and Client, and show me which children get forced into client rendering when I flip a parent.
```

**Hydration:**

```text
Build me an interactive demo showing the server HTML on the left, the client React tree on the right, and a Hydrate button I can click to see them sync up. Then let me intentionally cause a mismatch and watch the hydration error happen.
```

**Streaming with Suspense:**

```text
Build me a mock Next.js page with three components (fast, medium, slow) wrapped in Suspense. Click load and let me watch each component stream in over real seconds with skeletons swapping to content. Add a toggle to compare with all Suspense removed.
```

**Caching layers:**

```text
Build me an interactive diagram of a Next.js request flowing through the four caching layers. Let me toggle each cache hit or miss and watch the request shortcut or go all the way to the database.
```

**Server Actions:**

```text
Build me an interactive Server Action demo. Show a form on the left, the server function on the right, and animate the data flowing across when I submit. Then trigger revalidatePath and show a cached area refreshing.
```

**Dynamic vs static rendering:**

```text
Build me an interactive Next.js page with toggles for cookies, headers, searchParams, and noStore. Show a live Render Mode badge that flips between Static and Dynamic, and explain which toggle caused the flip.
```

**App Router file conventions:**

```text
Build me an interactive App Router folder where I can click each special file (layout, page, loading, error, etc.) and see exactly where and when it renders in the final page. Grey out the others so I can isolate one at a time.
```

---

## Learning Fundamentals

**HTML/CSS playground:**

```text
Show me flexbox vs grid for a card layout, side by side, and let me tweak gap and alignment values.
```

**CSS animations and transitions:**

```text
Build a hover effect, a loading spinner, and a modal slide-in on one page so I can see them all run.
```

**JavaScript concept demo:**

```text
Build a small interactive page that demonstrates closures, the event loop, async/await, and debouncing.
```

**DOM manipulation drill:**

```text
Build a to-do list using only vanilla JS, no frameworks. Then add localStorage, drag-to-reorder, and filters.
```

**Responsive design practice:**

```text
Build me a layout, then make it mobile-first and show the breakpoints in action.
```

---

## Frontend Framework Practice

**Reusable React component:**

```text
Build a reusable Button component with variants.
```

**Controlled form:**

```text
Show me a controlled form with validation.
```

**Hooks deep-dive:**

```text
Build a page that demos useState, useEffect, useMemo, and useReducer with visible side effects.
```

**State management comparison:**

```text
Build a counter with React Context, then refactor it to Zustand and Redux Toolkit. Compare all three styles side by side.
```

**Tailwind speedrun:**

```text
Rebuild a real site's hero section using only Tailwind. Help me iterate on spacing and colors until it matches.
```

---

## Backend and API

**Express route sketch:**

```text
Draft Express route handlers, middleware, and error handling in one file I can refine.
```

**API client UI:**

```text
Build an HTML page that hits the PokeAPI and renders results, with fetch, loading, and error states.
```

**SQL practice:**

```text
Write me schemas and queries as a working document. Help me refine table relationships, add indexes, and explain the query plans.
```

**Auth flow sketch:**

```text
Sketch JWT vs session and OAuth flows as runnable mock code, not abstract diagrams.
```

---

## Portfolio-Grade Mini Projects

**Startup landing page:**

```text
Build a landing page for a fake startup. Help me iterate on copy, layout, and CTAs until it looks shipped.
```

**Single-page resume site:**

```text
Build my resume as a single-page site I can export and host on GitHub Pages.
```

**Pricing page mockup:**

```text
Build a pricing page mockup.
```

**Login page mockup:**

```text
Build a login page mockup.
```

**Dashboard mockup:**

```text
Build a dashboard mockup.
```

**Weather app:**

```text
Build a weather app.
```

**Currency converter:**

```text
Build a currency converter.
```

**Markdown previewer:**

```text
Build a markdown previewer.
```

**Tip calculator:**

```text
Build a tip calculator.
```

**Portfolio gallery component:**

```text
Build a portfolio gallery component I can drop into my real site later.
```

---

## Study and Interview Prep

**LeetCode walkthrough:**

```text
Give me a brute-force solution to this problem, then optimize it step by step. Keep both versions visible.
```

**Data structures cheat sheet:**

```text
Build me a cheat sheet for linked list, hashmap, and binary tree operations with time complexities.
```

**System design one-pager:**

```text
Design a URL shortener. Include the diagram-in-text, API design, schema, and tradeoffs in one doc.
```

**HTTP status code reference:**

```text
Build me a personalized HTTP status code reference, with notes on when I would actually use each.
```

**Git command reference:**

```text
Build me a personalized Git command reference, organized by the situations I actually run into.
```

**Linux command reference:**

```text
Build me a personalized Linux command reference, focused on the commands I use daily.
```

**Mock interview question bank:**

```text
Build me a mock interview question bank organized by topic.
```

---

## Documentation and Writing

**Project README:**

```text
Draft me a README with installation, usage, screenshot placeholders, and contributing sections.
```

**Learning blog post:**

```text
Help me turn what I learned about CORS today into a blog post. Outline first, then expand.
```

**Class project proposal:**

```text
Draft a project proposal with problem, solution, tech stack, and milestones.
```

**API documentation:**

```text
Help me write API documentation for my backend project.
```

---

## Tooling for Your Workflow

**Personal study tracker:**

```text
Build me a personal study tracker for topics covered, projects shipped, and courses in progress.
```

**Learning roadmap:**

```text
Build me a learning roadmap doc that I can evolve as I discover what to learn next.
```

**Mini utilities (regex tester, JSON formatter, color palette):**

```text
Build me a regex tester, JSON formatter, and color palette explorer as small utilities.
```

**Boilerplate generator:**

```text
Give me a Vite + React + Tailwind + TypeScript starter file structure.
```
