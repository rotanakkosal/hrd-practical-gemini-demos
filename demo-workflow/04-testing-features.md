# Stage 4 — Stress-Test Antigravity 2.0's Full Capabilities

**Goal:** Build Spendly *and* exercise every major Antigravity 2.0 feature at the same time.
**Time:** 1–3 hours
**Output:** A working app + a real, lived sense of what Antigravity 2.0 can do.

---

## Why This Workflow Exists

The simple 3-message workflow in `03-antigravity.md` is the fastest path to a working app — but it doesn't push Antigravity 2.0 hard. This workflow does. Each phase deliberately uses a different capability so you learn the tool's range.

---

## The 8 Phases

### Phase 1 — Plan with guardrails
**Capability tested:** Plan-then-execute

> Read `PRD.md`, `DESIGN.md`, and the screens in `/design-reference`. Plan how you'd build the full Spendly app. Show me the plan as a task tree before writing any code. Identify which tasks can run in parallel and which must be sequential.

✅ **What to watch:** Does it correctly identify parallelizable work? Is the plan reasonable? Reject and iterate if not.

---

### Phase 2 — Foundation build
**Capability tested:** Single-agent end-to-end task

> Go ahead with just the foundation: project scaffold, database schema, auth, and the base layout (sidebar + top bar). Stop and show me before building any pages.

✅ **What to watch:** Does one agent handle the whole foundation cleanly? Any setup errors? How long?

---

### Phase 3 — Dashboard with MCP + browser verification
**Capability tested:** Multi-tool chaining

> Build the dashboard page next. Use the Stitch MCP to re-fetch the dashboard design and match it exactly. When done, open the dev server in the integrated browser, take a screenshot, and compare it visually to `/design-reference/dashboard.html`. Report any visual differences.

✅ **What to watch:** Does it actually use the Stitch MCP? Does the browser screenshot match the reference?

---

### Phase 4 — Parallel page generation
**Capability tested:** Multi-agent orchestration (THE killer feature)

> Now build the four remaining pages in parallel. Dispatch four agents simultaneously, one per page:
>
> - Agent A: Transactions page (full sortable table)
> - Agent B: Budgets page (set/edit monthly budgets)
> - Agent C: Reports page (charts and trends)
> - Agent D: Settings page (theme, currency, categories)
>
> Each agent matches the corresponding HTML in `/design-reference/`. Each appends its summary to `AGENT_LOG.md` when finished. They must not touch each other's files.

✅ **What to watch:** Open the Agent Manager. Watch four progress streams at once. Time it vs sequential.

---

### Phase 5 — Theme toggle with subagents
**Capability tested:** Dynamic subagents (agents spawning agents)

> Add a light/dark theme toggle to the app. Plan the work first, then spawn subagents to update each component in parallel — one subagent per component. Show me the subagent tree before executing.

✅ **What to watch:** Does it spawn 8–15 child agents? Does the tree visualization show the hierarchy clearly?

---

### Phase 6 — Autonomous QA pass
**Capability tested:** Browser-driven testing

> Open the running app. Create a test user. Log five fake transactions across different categories. Set a $200 budget on "Food." Now log a $250 food expense. Verify:
> - The over-budget warning appears
> - The donut chart updates correctly
> - The recent transactions list shows the new entry
> - The total matches the sum of the five transactions
>
> Report any bugs as a checklist.

✅ **What to watch:** Does the agent actually click through the UI like a user would? Does it find real bugs?

---

### Phase 7 — Parallel bug fixes
**Capability tested:** Parallel agents on small tasks

> Based on the bug list from the QA pass, fix every bug in parallel. Assign one agent per bug. Each must verify its fix in the browser before declaring done.

✅ **What to watch:** How well do many small parallel agents coexist? Any merge conflicts?

---

### Phase 8 — Polish with the full MCP chain
**Capability tested:** End-to-end MCP workflow

> Run three agents in parallel:
> - Agent 1: Generate a favicon and OG image matching the brand from `DESIGN.md`, place them in `/public`, and wire them up in the layout.
> - Agent 2: Use Stitch MCP to check if there are any newer designs I've made since the last fetch. If yes, update the corresponding pages.
> - Agent 3: Add proper loading and empty states to every page.

✅ **What to watch:** Does Stitch MCP find updates? Does each agent stay in its lane?

---

## What You'll Learn

| Phase | Capability tested | What it reveals |
|---|---|---|
| 1 | Planning | How well the agent reasons about your project |
| 2 | Single-agent work | Baseline quality of one agent on a meaty task |
| 3 | MCP + browser chain | Whether tools actually compose end-to-end |
| 4 | Parallel agents | The headline 2.0 feature in real conditions |
| 5 | Subagents | Whether the hierarchy is real or marketing |
| 6 | Autonomous testing | Whether agents can find their own bugs |
| 7 | Parallel small tasks | Coordination overhead vs. payoff |
| 8 | Full MCP chain | The "future of dev" pitch in practice |

---

## Things to Measure

- **Speed:** how long does a 4-agent parallel run take vs 4 sequential prompts?
- **Quality:** do parallel agents produce consistent output, or does each one's "style" drift?
- **Reliability:** how often does an agent get stuck or produce broken code?
- **Recovery:** how well does it diagnose its own failures?
- **Token cost:** does the cost panel match what you expected?

---

## Bonus: Test Recovery from Failure

After your app is working, deliberately break it:

> Delete the entire `/app/api/transactions` folder, then act as if I just reported: "The transactions page is broken. Find what's wrong and fix it."

This tests autonomous debugging. Does it discover the missing API, recreate it from scratch (or from the Stitch design), and verify the page works again?

---

## Bonus: Test the Antigravity CLI (if installed)

The CLI is separate from the desktop app (Go-based, faster). Run a task from the terminal:

```bash
antigravity run "Generate API documentation for the entire backend"
```

Tests the headless/scriptable interface — useful for CI pipelines.

---

## Honest Recommendation for First-Time Testers

If you only have time for **three phases**, run:

1. **Phase 4** (parallel agents) — the headline feature, biggest "wow"
2. **Phase 6** (autonomous QA) — most useful day-to-day capability
3. **Phase 1** (planning guardrails) — most important to verify before trusting on bigger projects

Everything else is bonus.
