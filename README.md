# getitassist.info — Cloudflare Pages Deployment

## Files
- `index.html` — Main website
- `_headers` — Cloudflare security headers
- `_redirects` — www redirect + SPA fallback

## Deploy to Cloudflare Pages

### Option 1 — Drag & Drop (fastest)
1. Go to https://dash.cloudflare.com → Pages
2. Click **Create a project** → **Direct Upload**
3. Drag the entire `getitassist.info/` folder
4. Set project name: `getitassist`
5. Click **Deploy**

### Option 2 — GitHub (recommended for ongoing updates)
1. Push this folder to a GitHub repo
2. In Cloudflare Pages → **Connect to Git**
3. Select your repo, set build output = `/` (root)
4. No build command needed (pure static HTML)
5. Deploy

### Custom Domain
1. In your Cloudflare Pages project → **Custom Domains**
2. Add `getitassist.info`
3. Cloudflare will auto-configure DNS if your domain is on Cloudflare

### Environment
- No build tools needed — pure static HTML/CSS/JS
- No Node.js or npm required
- Works on Cloudflare Pages free tier
