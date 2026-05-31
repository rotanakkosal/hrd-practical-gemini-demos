# 02 — Stitch Prompt

Tool: [stitch.withgoogle.com](https://stitch.withgoogle.com)

> ⚠️ Before submitting:
> - Toggle to **Web / Desktop mode** (not mobile)
> - Switch to **Experimental / Pro mode** for better quality
> - **Attach your favorite Variant screenshot** as a reference image — non-negotiable for style consistency

---

## ⭐ Main prompt (with Variant screenshot attached)

```
Build a desktop web app called Spendly — a personal expense tracker designed for daily use on a 1440px-wide browser window. The attached reference image defines the visual direction.

Visual style (anchor to reference image): Dark theme with deep charcoal/black backgrounds, high contrast white/light text. Monospace font (JetBrains Mono) for all financial figures, dates, and tabular numbers. Sans-serif (Inter) for UI labels, headings, body text. Color-coded category system using muted/desaturated tones — purple, green, blue, orange, yellow. Status indicators as small colored dots — green for cleared, orange for pending, red for over budget. Conic gradient donut chart for category breakdown. Compact 8px grid spacing, dense and calm information architecture.

Layout (three-panel on Dashboard): Left sidebar ~240px with logo, ⌘K search, nav items (Dashboard, Transactions, Budgets, Reports, Inbox), user profile at bottom. Center main area with month picker top bar, large total-spent card, recent transactions table. Right meta panel ~280px with category donut and budget progress bars.

Screens to generate:
1. Dashboard — total spent this month, vs-last-month comparison, monthly budget remaining, recent transactions table (6–8 rows), category donut, budget progress bars
2. Transactions — full-width sortable table (Date, Payee, Category, Amount, Status), filter bar, search, bulk select checkboxes, CSV export button
3. Budgets — list of all budgets per category with monthly limits, progress bars, edit controls, over-budget warning states
4. Reports — 6-month spending trend line chart, category breakdown stacked area, top merchants list, month-over-month comparison
5. Add Transaction modal — large amount input, category selector with colored badges, date picker, payee field, notes, optional receipt upload
6. Settings — sections for account, preferences (theme, currency), categories management, data export

Interaction details: Hover states on rows and buttons. Keyboard shortcuts ⌘K for search, N for new transaction, / for filter. Inline editing in the transactions table. Three-dot action menus on rows. Smooth, restrained transitions — no flashy animations. Aesthetic inspired by Linear, Notion, and Stripe Dashboard.
```
---

## After we're happy

1. Name our Stitch project clearly (e.g., **"Spendly Expense Tracker"**), we'll reference this exact name in Antigravity
2. Get our Stitch API key: Profile picture → **Stitch Settings** → **API key** → **Create key** → **copy immediately**