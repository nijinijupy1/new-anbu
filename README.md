# Anbu Cafee — Billing

Browser-only café billing POS. **No backend / no database server** — all data is saved in the browser with `localStorage`.

## How it works

- Runs in the browser (Chrome / Edge / etc.)
- Login, menu, cart, bills, sales, users, offers, and shop QR are stored locally
- Closing the browser keeps your data (same browser / same device)
- Clearing site data or using another browser starts fresh

## Run locally

```bash
npm install
npm run dev
```

Open the URL shown in the terminal (usually `http://localhost:5173`).

For a production build (static files only):

```bash
npm run build
npm run preview
```

## Features

- Login / logout (multi-user)
- Billing — tap item → cart, bill number, table & time
- Pay now (shop QR), print bill, KOT, WhatsApp bill
- Manage menu (CRUD + image upload)
- Bill track, offers (WhatsApp), users
- Daily & monthly sales reports (with print)

## Publish online (free)

### Option 1 — Netlify Drop (easiest, ~1 minute)
1. Open https://app.netlify.com/drop
2. Drag this folder onto the page:  
   `C:\Users\Niji__office\Desktop\Anbu_Cafee_Billing\dist`  
   Or drag: `Anbu_Cafee_Online.zip` from your Desktop
3. Netlify gives you a free HTTPS link (example: `https://random-name.netlify.app`)
4. Optional: create a free Netlify account to keep the site permanently and change the name

### Option 2 — Vercel
1. Go to https://vercel.com/new
2. Import your GitHub repo (or upload the project folder)
3. Click Deploy — free HTTPS URL in about a minute

### Option 3 — GitHub Pages
1. Push this project to GitHub
2. In repo **Settings → Pages**, publish from GitHub Actions / `dist`
3. Or connect the repo to Netlify/Vercel for auto-deploy on every push

**Note:** This app uses browser `localStorage` only — no server/database needed for hosting.

## Default login

- Username: `anbu`
- Password: `anbu@1010`

QR change password: `anbu@1010`
