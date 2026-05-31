# 03 — Antigravity 2.0 Prompts

Tool: [antigravity.google](https://antigravity.google)

Prereqs: Antigravity 2.0 installed, Stitch API key from Stage 2

---

### Verify

```
List my Stitch projects.
```

---

## ⭐ Simple 3-Message Workflow

### 1. Pull the Stitch design

```
Use the Stitch MCP to fetch my project named exactly "Spendly Expense Tracker". Save the design system into DESIGN.md and each screen's HTML/CSS into a design-reference folder.
```

> Use the **exact** project name from the `List my Stitch projects` output.

### 2. Describe the app and ask for a plan

```
I want to build a personal expense tracker called Spendly. Here's what it does:

- I log my daily expenses with an amount, category, date, and a short note
- It shows me my total spending this month and how it compares to last month
- I can set a monthly budget for each category and see warnings when I'm close to or over budget
- There's a transactions page with a sortable table
- There's a reports page with charts showing where my money goes
- It's just for me — no other users, no sharing

Use the design from DESIGN.md and the screens in design-reference as the visual style. Pick whatever modern web tech you think works best. Plan it first and show me the plan before building anything.
```

### 3. Approve the plan

```
Looks good, go ahead and build it.
```

Or correct it:

```
Looks good, but I don't need user accounts — it's only for me. Skip login.
```

### 4. See it run

```
Run the app and open it in the browser so I can see it.
```

---

## Iteration prompts

**Visual fixes**

```
The total spent number is too small — make it bigger.
```

```
The categories on the donut chart are hard to read. Add labels with category names and percentages.
```

```
The transactions table is missing the status column. Add it back.
```

**Feature additions**

```
Add a "duplicate transaction" button to each row in the transactions table.
```

```
Add a search bar at the top of the transactions page that filters as I type.
```

**Bug fixes**

```
When I try to set a budget, nothing happens. Open the app, try it yourself, and fix the bug.
```

```
The donut chart shows wrong percentages. They don't add up to 100%. Investigate and fix.
```

**Understanding what happened**

```
Explain what you just did in simple words.
```

```
I don't understand this error. Explain it in plain English and tell me how to fix it.
```

---

## Parallel agent prompts

**Build remaining pages in parallel**

```
Build the four remaining pages in parallel. Dispatch four agents simultaneously, one per page:

- Agent A: Transactions page (full sortable table)
- Agent B: Budgets page (set/edit monthly budgets)
- Agent C: Reports page (charts and trends)
- Agent D: Settings page (theme, currency, categories)

Each agent matches the corresponding HTML in /design-reference/. Each appends its summary to AGENT_LOG.md when finished. They must not touch each other's files.
```

**Polish pass in parallel**

```
In parallel:
- Agent 1: Add proper loading states (skeleton screens, not spinners) to every page
- Agent 2: Add empty states with friendly illustrations when there's no data
- Agent 3: Make sure every button has a hover and active state
```

**Visual polish in parallel**

```
In parallel:
- Agent 1: Generate a favicon and OG image matching the brand from DESIGN.md, place them in /public, and wire them up in the layout
- Agent 2: Use Stitch MCP to check for any newer designs and update affected pages
- Agent 3: Add proper page titles and meta descriptions to all pages
```

---

## Parallel vs sequential — rule of thumb

**Different files = parallel. Same file = sequential.**

When unsure, paste:

```
Can these tasks run in parallel? If yes, dispatch them as parallel agents. If no, explain what depends on what, then sequence them properly:

1. [task 1]
2. [task 2]
3. [task 3]
```

---

## When stuck

```
I'm stuck. The app isn't doing [X]. Walk me through what's happening, what you tried, and what we should do next. Use simple language.
```

---

## What's next

To stress-test all of Antigravity 2.0's features → `04-testing-features.md`