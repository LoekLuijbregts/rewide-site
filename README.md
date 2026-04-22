# Rewide.art — GitHub Repository

**Platform for fine art photography by people who actually went there.**  
Printed in Tilburg. Shipped across Europe.

---

## Repository structure

```
rewide-site/
├── index.html                          # Main platform homepage (self-contained)
├── README.md                           # This file
└── content/
    ├── photographers/
    │   ├── loek-luijbregts.md          # Profile + bio
    │   ├── leon-van-bon.md             # Profile + bio
    │   ├── ryan-le-garrec.md           # Profile + bio
    │   └── jop-hermans.md              # Profile + bio
    └── works/
        ├── loek-luijbregts-descriptions.md    # Product + social copy
        ├── leon-van-bon-descriptions.md        # Product + social copy
        ├── ryan-le-garrec-descriptions.md      # Product + social copy
        └── jop-hermans-descriptions.md         # Product + social copy
```

---

## Deploy to Netlify

### Option A — Netlify Drop (fastest, no account needed)
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag the entire `rewide-site` folder onto the page
3. Netlify gives you a live URL instantly

### Option B — GitHub + Netlify (recommended for ongoing updates)
1. Create a new GitHub repository: `rewide-site`
2. Upload all files (drag & drop on GitHub works fine)
3. Go to [app.netlify.com](https://app.netlify.com)
4. Click **Add new site → Import an existing project**
5. Connect GitHub, select `rewide-site`
6. Build settings: leave empty (static HTML, no build needed)
7. Click **Deploy site**

### Connect custom domain (rewide.art)
After deploy:
1. In Netlify: **Domain settings → Add custom domain → rewide.art**
2. Netlify gives you nameservers (e.g. `dns1.p01.nsone.net`)
3. In your domain registrar: point nameservers to Netlify's
4. SSL certificate is automatic (Let's Encrypt)

---

## Content workflow

Each photographer has two files:
- `photographers/[name].md` — biography and profile for the photographer page
- `works/[name]-descriptions.md` — ready-to-use copy including:
  - Product page descriptions (SEO-optimised)
  - Instagram captions (NL + EN)
  - Story versions (short format)

To add a new work:
1. Add the image to `index.html` (base64 or hosted URL)
2. Add product description + captions to the photographer's descriptions file
3. Redeploy

---

## Next development priorities

- [ ] Wall preview tool — real photo upload + overlay
- [ ] Mollie payment integration
- [ ] Individual photographer pages (`/loek`, `/leon`, etc.)
- [ ] Work detail pages (`/works/ugandese-highlands`)
- [ ] Order management system
- [ ] Photographer dashboard (upload, track sales)

---

## Photographers

| Photographer | Style | Prints |
|---|---|---|
| Loek Luijbregts | Adventure · Culture · Cycling | 14 |
| Léon van Bon | Racing · Sport · Emotion | 22 |
| Ryan Le Garrec | Ultra · Bikepacking · Documentary | 18 |
| Jop Hermans | Ocean · Surf · Fine Art | 31 |

---

## Contact

hello@rewide.art  
Printed by Printservice Tilburg, Tivolistraat, Tilburg NL
