# BizEco — Business, Simplified.

A local-first business operations and intelligence demo for Albanian small and medium-sized businesses. This standalone first version runs directly in a modern browser and needs no package install, API key, or server.

## Run it

Open `index.html` in a current desktop or mobile browser. The demo workspace is fictional and is saved in that browser with `localStorage`. Use **Reset demo data** in Settings to restore the original sample records.

## What works in this build

- Dark BizEco dashboard with revenue, expenses, management-result estimate, sample margin, charts, and data-derived stock observations.
- Sales, customers, products, expenses, and marketing record creation.
- Browser-local persistence for workspace settings and edits.
- Search/filter for sales, customer, product, and expense tables.
- Inventory threshold indicators and editable automation rules (local configuration only).
- Deterministic local advisor responses for recorded revenue, expenses, and stock.
- CSV exports for major record lists and a combined sales/expense export.
- Responsive navigation and mobile layout.
- ALL, EUR, and USD workspace display preference. Original record currencies are retained; this demo does not perform exchange-rate conversion.

## Honest limitations

This is a browser-only prototype, not a production SaaS backend. It has no sign-in, PostgreSQL database, tenant isolation, server-side authorization, scheduled/background jobs, real email/bank/e-commerce integrations, legally compliant invoicing, AI provider, or audited stock movement ledger. Local browser storage is not a secure shared database and can be cleared by the browser. Seed figures are fictional and should not be interpreted as real business accounts. Analytics trend chart is illustrative rather than derived daily history.

The management result is recorded sales less recorded expenses for the current sample workspace; it is not a certified accounting statement and does not apply tax or accrual accounting.

## Files

- `index.html` — app shell and navigation.
- `styles.css` — responsive deep-black and Alpine-green design system.
- `app.js` — demo data, local workflows, calculations, chart drawing, and CSV export.
- `assets/bizeco-logo.png` and `assets/bizeco-wordmark.svg` — supplied brand artwork and cropped wordmark display.

## Next production steps

For real users and sensitive business records, migrate persistence to an authenticated server application backed by PostgreSQL; add server-side business scoping and permissions, database migrations, auditable inventory movements, accounting-reviewed metric definitions, import validation, automated tests, secure backups, and provider integrations only after credentials and access are configured.
First launch presents two workspace options: open the labeled fictional demo account, or create a workspace using your business name, type, country, currency, size, and primary goal. The personal-business option starts with no sample business records. You can return to workspace selection from Settings.
