# Netlify Deployment Guide

## Frontend-Only Deployment (Recommended for Netlify)

This project is configured to deploy the **frontend only** to Netlify as a static site.

### Steps to Deploy:

1. **Push to GitHub/GitLab**
   ```bash
   git add .
   git commit -m "Ready for Netlify deployment"
   git push origin main
   ```

2. **Connect to Netlify**
   - Go to [Netlify](https://netlify.com)
   - Click "Add new site" → "Import an existing project"
   - Connect your Git repository

3. **Configure Build Settings**
   - **Build command**: `npm run build`
   - **Publish directory**: `dist/public`
   - Click "Deploy site"

### Environment Variables (if needed)

If your app needs backend functionality, you'll need to:
- Deploy the backend separately (e.g., on Render, Railway, or Heroku)
- Add the backend API URL as an environment variable in Netlify

### Local Testing

Test the build locally before deploying:
```bash
npm run build
```

The built files will be in `dist/public` folder.

---

**Developed by Phumeh 2025**
