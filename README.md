# RBPT Staff Forms

Online claim forms for The Station Richmond staff — mileage and expense claims.

## Pages

- `index.html` — hub / home page
- `mileage.html` — mileage claim form
- `expenses.html` — expense claim form

## Deploy to GitHub Pages (5 minutes)

1. Go to [github.com](https://github.com) and sign in (or create a free account)
2. Click **New repository** — `name it `rbpt-forms` (or anything you like)
3. Set it to **Public**, then click **Create repository**
4. Upload `index.html`, `mileage.html`, and `expenses.html` using the **Add file → Upload files** button
5. Go to **Settings → Pages**
6. Under **Source**, select `main` branch and click **Save**
7. Your site will be live at `https://YOUR-USERNAME.github.io/rbpt-forms/`

## Connect email submissions (Formspree)

Forms are wired to send via [Formspree](https://formspree.io) — free for up to 50 submissions/month.

1. Go to [formspree.io](https://formspree.io) and create a free account
2. Click **New Form** ℔ give it a name (e.g. "RBPT Mileage")
3. Set the recipient email to the Chief Executive's address
4. Copy the endpoint URL (looks like `https://formspree.io/f/xyzabc`)
5. In `mileage.html`, find the line:
   ```
   const ENDPOINT = 'https://formspree.io/f/YOUR_ENDPOINT';
   ```
   Replace `YOUR_ENDPOINT` with your actual ID (e.g. `xyzabc`)
6. Do the same in `expenses.html`
7. Re-upload both files to GitHub

Repeat step 2–4 to create a **second form** for expenses if you want them going to different email addresses.

## Expense policy

The expense policy displayed in `expenses.html` is a draft — review and amend it with the Chief Executive before going live. Key points to confirm:
- The £5 receipt threshold
- The £50 pre-approval threshold  
- The 30-day submission window
- Whether alcohol can ever be claimed (e.g. for events)
