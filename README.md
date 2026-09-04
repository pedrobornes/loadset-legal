# loadset-legal

Public legal documents for **LoadSet** (GitHub Pages).

**Owner:** Pedro Antonio Bornes Durán  
**Contact:** info@status-timer.com  
**Language:** English (single source of truth for Google Play / global users)

## Published URLs

| Document | URL |
|----------|-----|
| Index | https://pedrobornes.github.io/loadset-legal/ |
| Privacy | https://pedrobornes.github.io/loadset-legal/privacy.html |
| Terms | https://pedrobornes.github.io/loadset-legal/terms.html |
| Legal notice | https://pedrobornes.github.io/loadset-legal/legal.html |

## App configuration (LoadSet)

In `loadset/frontend/.env`:

```env
VITE_LEGAL_PRIVACY_URL=https://pedrobornes.github.io/loadset-legal/privacy.html
VITE_LEGAL_TERMS_URL=https://pedrobornes.github.io/loadset-legal/terms.html
VITE_LEGAL_NOTICE_URL=https://pedrobornes.github.io/loadset-legal/legal.html
VITE_LEGAL_CONTACT_EMAIL=info@status-timer.com
```

## Editing

1. Update `legal.config.json` as a local reference (HTML is already filled).
2. Edit the `.html` files directly for content changes.
3. Before monetisation: review texts with a professional if the business model changes.

## Publishing

```bash
git add -A
git commit -m "Update legal texts"
git push
```

GitHub Pages serves from `main` (short delay after push).
