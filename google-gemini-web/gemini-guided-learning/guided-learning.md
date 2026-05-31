# Guided Learning

A prompt library for step-by-step, interactive learning. Each prompt walks you through a concept in stages, with practice exercises or quizzes between steps so you can confirm understanding before moving on.

---

**React Hooks one at a time:**

```text
Walk me through React Hooks one at a time. Start with useState and build a counter together. Then useEffect with a fetch example. Then useReducer with a small todo. Keep all examples visible side by side so I can compare. After each hook, give me a small exercise and don't move on until I solve it.
```

**SQL query building:**

```text
Teach me SQL by building one query step by step. Start with SELECT and show me the full table. Add a WHERE and show the filtered result. Add a JOIN and show the wider result. Add GROUP BY and show the aggregated result. After each clause, give me a small puzzle to solve.
```

**Git workflow visually:**

```text
Teach me Git by showing me an animated commit graph that updates as I run commands. Start with git init and an empty graph. Walk me through commit, branch, merge, and rebase, animating the graph after each step. Let me predict what the graph will look like before each command runs.
```

**The request lifecycle:**

```text
Teach me what happens when I type a URL and hit enter. Build me an animated journey through DNS lookup, TCP handshake, HTTPS, HTTP request, server processing, response, and browser render. Pause at each stage so I can click for more detail before moving on.
```

**CSS layout progression:**

```text
Walk me through CSS layout from the ground up. Start with normal document flow and show me a page with no CSS. Add display block vs inline. Then floats. Then flexbox. Then grid. At each stage, give me a layout puzzle to solve before moving on.
```

**Async JavaScript progression:**

```text
Walk me through async JavaScript in stages. First show me a fetch using callbacks with full callback hell. Then rewrite it using promises and chaining. Then rewrite it again using async/await. Keep all three versions side by side so I can compare. Quiz me on what each version outputs before revealing.
```

**Debugging practice with a broken app:**

```text
Build me a small Next.js app with five intentional bugs — a hydration error, a missing use client, wrong props passing, a null reference, and a missing env variable. Walk me through finding each one. Show me the error, ask what I think is wrong, let me try a fix, then reveal the correct fix.
```

**Database schema design from a messy spreadsheet:**

```text
Teach me database schema design by walking me through normalizing a messy spreadsheet into 3NF. Show me the spreadsheet with all its problems. Walk me through each normal form (1NF, 2NF, 3NF) step by step. At each stage, ask me to identify the violations before showing the answer.
```

**Authentication flow piece by piece:**

```text
Teach me authentication by building it up piece by piece. Start with the simplest case: a hardcoded password check. Then add session storage. Then add a database. Then add password hashing. Then add JWT tokens. At each step, explain what attack the new piece protects against. Quiz me on the differences before moving on.
```

**Recursion with call stack visualization:**

```text
Teach me recursion by visualizing the call stack. Start with a simple factorial. Show me stack frames pushing on as the function calls itself, then popping off as each one returns a value. Let me step forward and backward through each call. Then try fibonacci and let me see the explosion of redundant calls.
```
