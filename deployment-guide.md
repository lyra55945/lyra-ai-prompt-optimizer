# Lyra AI Prompt Optimizer - Deployment Guide

## Option 1: Vercel (Recommended - Free & Easy)

### Steps:
1. **Create Vercel Account**: Go to https://vercel.com and sign up
2. **Connect GitHub**: Link your GitHub account to Vercel
3. **Push to GitHub**: 
   ```bash
   git init
   git add .
   git commit -m "Initial commit - Lyra AI Prompt Optimizer"
   git branch -M main
   git remote add origin https://github.com/yourusername/lyra-ai-optimizer.git
   git push -u origin main
   ```
4. **Deploy on Vercel**:
   - Go to Vercel dashboard
   - Click "New Project"
   - Import your GitHub repository
   - Add environment variable: `NEXT_PUBLIC_OPENROUTER_API_KEY`
   - Click Deploy

**Result**: Your app will be live at `https://your-project-name.vercel.app`

---

## Option 2: Netlify (Alternative)

### Steps:
1. **Create Netlify Account**: Go to https://netlify.com
2. **Build the project**:
   ```bash
   npm run build
   npm run export  # if using static export
   ```
3. **Deploy**:
   - Drag and drop the `out` folder to Netlify
   - Or connect GitHub repository
   - Add environment variables in Netlify dashboard

---

## Option 3: Railway (Backend-friendly)

### Steps:
1. **Create Railway Account**: Go to https://railway.app
2. **Connect GitHub**: Link your repository
3. **Deploy**: Railway auto-detects Next.js and deploys
4. **Add Environment Variables**: Set `NEXT_PUBLIC_OPENROUTER_API_KEY`

---

## Option 4: DigitalOcean App Platform

### Steps:
1. **Create DigitalOcean Account**: Go to https://digitalocean.com
2. **Create App**: Use App Platform
3. **Connect Repository**: Link GitHub/GitLab
4. **Configure**: Set build command and environment variables
5. **Deploy**: Automatic deployment

---

## Important Notes:

### Environment Variables:
For any platform, you'll need to set:
```
NEXT_PUBLIC_OPENROUTER_API_KEY=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
```

### Security Considerations:
- The API key is exposed in the frontend (NEXT_PUBLIC_)
- Consider implementing a backend API route for production
- Monitor API usage to prevent abuse

### Custom Domain (Optional):
- Most platforms allow custom domain setup
- Purchase domain from providers like Namecheap, GoDaddy
- Configure DNS settings in your deployment platform

---

## Quick Start with Vercel (5 minutes):

1. **Install Vercel CLI**:
   ```bash
   npm i -g vercel
   ```

2. **Deploy directly**:
   ```bash
   vercel
   ```

3. **Follow prompts**:
   - Login to Vercel
   - Set project name
   - Add environment variable when prompted

4. **Your app is live!** 🎉

---

## Production Optimization:

### For better security, create an API route:
```javascript
// pages/api/optimize.js or app/api/optimize/route.js
export async function POST(request) {
  const apiKey = process.env.OPENROUTER_API_KEY; // Server-side only
  // ... API logic here
}
```

### Update client to use your API:
```javascript
// Instead of calling OpenRouter directly
const response = await fetch('/api/optimize', {
  method: 'POST',
  body: JSON.stringify(promptData)
});
```

This keeps your API key secure on the server side.
