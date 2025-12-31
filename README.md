# Website

Built with [LiteShow](https://liteshow.io) - AI-first, Git-powered CMS

## Quick Deploy

Choose your preferred hosting platform:

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/coverdashllc/liteshow-website#LITESHOW_PROJECT_SLUG=website&LITESHOW_API_URL=https://api.liteshow.io)

[![Deploy to Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/coverdashllc/liteshow-website&env=LITESHOW_PROJECT_SLUG,LITESHOW_API_URL&envDescription=Required%20environment%20variables)

**Your project slug:** `website` (copy and paste when prompted during deployment)

After deploying, any content you publish in LiteShow will automatically trigger a rebuild.

## Manual Setup

If you prefer manual setup:

1. Import this repo in your hosting platform
2. Set build command: `pnpm install && pnpm build`
3. Set publish directory: `dist`
4. Add these **required** environment variables:
   - `LITESHOW_PROJECT_SLUG` = `website`
   - `LITESHOW_API_URL` = `https://api.liteshow.io`

## Environment Variables

**Both environment variables are required for deployment:**

- `LITESHOW_PROJECT_SLUG` - Your project slug: `website`
- `LITESHOW_API_URL` - LiteShow API endpoint: `https://api.liteshow.io`

The site fetches your published content from the LiteShow API at build time.

## Local Development

```bash
# Copy environment template
cp .env.example .env

# Edit .env and add your configuration
# LITESHOW_PROJECT_SLUG=website
# LITESHOW_API_URL=https://api.liteshow.io

# Install and run
pnpm install
pnpm dev
```

Visit http://localhost:4321

## How It Works

This Astro site fetches your published content from the LiteShow API at build time. LiteShow handles all the database infrastructure - you just manage your content!
