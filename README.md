# Shary & Co — Azerbaijan Medical University Landing Page

Marketing landing page for the **Dual Degree MBBS/MD + MPH** program at Azerbaijan
Medical University. Built with TanStack Start + React 19 + Tailwind v4 + shadcn/ui.

The homepage (`/`) is the campaign landing page: explainer video → credibility →
fee breakdown → "Check Eligibility" form. On submit it fires the Meta Pixel `Lead`
event, posts the lead to your CRM webhook, and opens WhatsApp with a pre-filled message.

## Run it
```bash
npm install
npm run dev      # http://localhost:8080
npm run build
```

## Configure (env vars)
| Variable | Purpose |
|---|---|
| `VITE_META_PIXEL_ID` | Turns the Meta Pixel on (PageView + Lead). Public, client-side. |
| `LEAD_WEBHOOK_URL` | Server-side webhook that receives each lead (e.g. Zapier/Make → Google Sheets). |

## Edit later (search the code for `EDIT:`)
- `VIDEO_EMBED_URL` in `src/routes/index.tsx` — paste your explainer video embed URL.
- Credibility image slots — drop photos in `/public` and fill the `stories` array.
- Footer privacy-policy link — add a real page (required for Meta ads).
