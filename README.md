# Moliam Brand Site

Elite AI Infrastructure & Digital Growth - Company Website

## Automated Deployment

This site deploys automatically to Cloudflare Pages via GitHub Actions on every push to main.

### Setup Instructions

1. **Create GitHub Repository**
   ```bash
   git remote add origin https://github.com/oscarsolis3301/moliam-brand.git
   git push -u origin main
   ```

2. **Add GitHub Secrets**
   Go to Repository Settings → Secrets and variables → Actions
   
   Add these secrets:
   - `CLOUDFLARE_API_TOKEN` - Your Cloudflare API token
   - `CLOUDFLARE_ACCOUNT_ID` - `ea22c3650ec12091075256922c5a17b5`

3. **Required Token Permissions**
   - Account: Cloudflare Pages:Edit
   - Account: Cloudflare Workers:Edit
   - Zone: Zone:Read

### Deploying

- **Automatic**: Push to `main` branch triggers deployment
- **Manual**: Go to Actions tab → Deploy to Cloudflare Pages → Run workflow

### Project Structure

```
.
├── index.html          # Main website
├── .github/
│   └── workflows/
│       └── deploy.yml  # GitHub Actions workflow
└── README.md          # This file
```

## Site Features

- Hero section with live metrics
- Services showcase (6 cards)
- API documentation preview
- Contact CTA
- Dark theme with gold accents
- Mobile responsive

## Local Development

Open `index.html` in any browser for local preview.

No build step required - pure HTML/CSS/JS.