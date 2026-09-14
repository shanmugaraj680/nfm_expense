# NFM Expense — PERSONAL LEDGER

Cloud-synced personal expense tracker for GitHub Pages + Supabase.

## Supabase project
- Project: `nfm_expense`
- Region: Mumbai (`ap-south-1`)
- URL: `https://nfxgifqgohcclmpsktqj.supabase.co`

## First-time setup
1. Open the Supabase project.
2. Create a Storage bucket named `expense-bills` and make it public, or run the Storage section at the bottom of `schema.sql` in SQL Editor.
3. Copy the project's **publishable key**.
4. Open `config.js` in this repository and replace `PASTE_YOUR_SUPABASE_PUBLISHABLE_KEY_HERE` with that publishable key. Never use a `service_role` or secret key in the browser.
5. Enable GitHub Pages for the `main` branch and root folder.

## Login
The requested simple static login is:
- Username: `nfm2019`
- Password: `nfm2019*nfm2019`

This is intentionally a simple client-side login, not a secure authentication system. Do not use it for sensitive financial data.

## Features
- Dashboard, Expenses and Payments views
- Supabase as the primary cloud data source
- Mobile + desktop responsive layout
- Expense CRUD
- Bill/receipt image upload
- Loan and Chit Fund progress
- Monthly budget
- MoM Expense Ratio = current month expense / previous month expense × 100
- MoM Expense Change %
- No local database or offline data fallback

## Important
The GitHub Pages frontend uses the Supabase publishable key only. If Supabase is unavailable, the app shows a cloud error instead of pretending that data was saved.
