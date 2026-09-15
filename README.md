# Collector Strategy ($CLLCTR)

Official site. Static single-file — no build step.

## Deploy (Vercel)
1. vercel.com -> Add New Project -> import this repo
2. Framework preset: **Other**, no build command, output dir: root
3. Deploy

## Updating after each buy round
Edit the `CONFIG` block at the bottom of `index.html`:
- `contractAddress`, `buyUrl`, `xUrl`, `robloxItemUrl`, `rolimonsUrl`
- `stats` — hatsHeld, robuxSpent, avgBuyPrice, inventoryValue
- `purchases` — one entry per buy: `{ date, account, qty, price }`

Commit -> Vercel auto-deploys.
