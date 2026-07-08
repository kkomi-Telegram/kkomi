# Vercel Deployment Guide

This project is configured with Vercel Web Analytics.

## Prerequisites

- A Vercel account
- Vercel CLI installed: `npm i -g vercel`

## Deployment Steps

### 1. Deploy to Vercel

```bash
vercel deploy
```

Follow the prompts to link your project to Vercel.

### 2. Enable Web Analytics

1. Go to your Vercel dashboard
2. Navigate to your project's **Analytics** tab
3. Click the **Enable** button in the header
4. Web Analytics is now enabled!

### 3. Verify Analytics

After deploying:

1. Visit your deployed site
2. Open the browser's Developer Tools (F12)
3. Go to the Network tab
4. Filter by XHR/Fetch requests
5. Look for a request to `/_vercel/insights/view`
6. If you see this request, analytics is working correctly!

## Local Development

To test the site locally:

```bash
npm run dev
```

This will start a local server at http://localhost:3000

## Analytics Data

- Analytics data will appear in your Vercel dashboard after a few days of traffic
- You can view page views, visitors, and other metrics in the Analytics tab

## Configuration

The project includes:
- `@vercel/analytics` package installed
- Analytics script in `public/index.html`
- `vercel.json` configuration with analytics enabled

## Documentation

For more information, visit:
- [Vercel Web Analytics Documentation](https://vercel.com/docs/analytics/quickstart)
- [Vercel Analytics Features](https://vercel.com/docs/analytics)
