# Budget Tracker Pro+

Single-file web app: [budget-tracker.html](budget-tracker.html)

Overview
- Simple, client-side budget tracker that stores transactions in localStorage.
- Adds, lists and deletes transactions; shows totals and monthly charts.

How it works (key functions)
- [`addTransaction`](budget-tracker.html) — validates form and appends a transaction to localStorage.
- [`removeTransaction`](budget-tracker.html) — deletes a transaction by id and refreshes the UI.
- [`render`](budget-tracker.html) — re-renders transaction list and triggers totals/month selection and charts.
- [`updateTotals`](budget-tracker.html) — computes totals for income, expenses and balance.
- [`populateMonths`](budget-tracker.html) — builds the month selector from transaction dates.
- [`updateCharts`](budget-tracker.html) — builds the bar and pie charts for monthly income/expenses and category breakdown.

Business problem solved
- Provides a low-friction way for individuals or small teams to track cash flow and spending categories locally (no backend required).
- Supports quick decision-making by summarizing:
  - Total income and expenses.
  - Monthly breakdown and category distribution (visualized with charts).
- Helps answer business questions like:
  - "Are we operating at a surplus or deficit this month?" — computed as $balance = income - expense$.
  - "Which categories consume the most budget this month?" — shown by the category pie chart.

Quick math (how balance is calculated)
$$
balance = income - expense
$$

How to use
1. Open [budget-tracker.html](budget-tracker.html) in a modern browser.
2. Add transactions via the form (positive amounts = income, negative = expenses).
3. Use the month selector to view monthly summaries and charts.
4. Transactions persist in browser localStorage.

Why this is useful for business
- No infrastructure cost or setup; ideal for freelancers, micro-businesses, or early-stage projects.
- Fast insights into monthly cash flow and categorical spending to prioritize cost-saving or investment decisions.
- Export or extend: the single-file app is easy to port, integrate with a backend, or add export/import features.

Files
- [budget-tracker.html](budget-tracker.html) — full application code (UI, storage, and charting).
```// filepath: README.md
