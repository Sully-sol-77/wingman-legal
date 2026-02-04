# Wingman Legal Pages

Static HTML pages for Apple App Store review requirements (Privacy Policy, Terms of Service, and Support).

## Purpose

This repository contains reviewer-proof static pages required for App Store submission:
- Privacy Policy (`/privacy`)
- Terms of Service (`/terms`)
- Support (`/support`)

All pages are plain HTML/CSS with no JavaScript dependencies, cookies, or external embeds.

## Local Preview

No build system required. Simply open the HTML files in your browser:

```bash
# Option 1: Open directly
open privacy.html
open terms.html
open support.html

# Option 2: Use a local server (recommended)
python3 -m http.server 8000
# Then visit http://localhost:8000
```

## Vercel Deployment

1. **Import Project**
   - Go to [Vercel Dashboard](https://vercel.com/dashboard)
   - Click "Add New" → "Project"
   - Import this repository

2. **Configure Settings**
   - **Framework Preset:** Other
   - **Build Command:** (leave empty)
   - **Output Directory:** (leave as default)
   - **Install Command:** (leave empty)

3. **Deploy**
   - Click "Deploy"
   - Your site will be live at `https://<project>.vercel.app`

## App Store Connect URLs

After deployment, use these URLs in App Store Connect:

- **Privacy Policy:** `https://<project>.vercel.app/privacy`
- **Terms of Service:** `https://<project>.vercel.app/terms`
- **Support:** `https://<project>.vercel.app/support`

Replace `<project>` with your Vercel project name.
