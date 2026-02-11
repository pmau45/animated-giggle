# AXIOM CANINE - Netlify Deployment Guide

## 📦 Quick Deploy to Netlify

### Option 1: Drag & Drop (Easiest)
1. Create a folder with these files:
   - `index.html`
   - `netlify.toml`
   - `success.html`
2. Go to [Netlify Drop](https://app.netlify.com/drop)
3. Drag the folder onto the page
4. Your site is live!

### Option 2: GitHub Integration (Recommended)
1. Push these files to your GitHub repository
2. Log in to [Netlify](https://app.netlify.com)
3. Click "Add new site" → "Import an existing project"
4. Connect to GitHub and select your repository
5. Netlify will auto-detect settings from `netlify.toml`
6. Click "Deploy site"

## 🎨 Adding Your Hero Image

To add your dog photo to the hero section:

1. Create an `images` folder in your project root
2. Add your hero image (recommended: 1920x1080px, optimized JPEG)
3. Name it `hero-dog.jpg`
4. In `index.html`, change this line:
   ```html
   <header class="hero">
   ```
   to:
   ```html
   <header class="hero with-image">
   ```

## 📧 Form Setup

The contact form is already configured for Netlify Forms. After your first deployment:

1. Go to your Netlify dashboard
2. Navigate to "Forms" tab
3. Configure email notifications
4. Optional: Set up form submission success redirect to `/success.html`

## 🔧 Custom Domain

To add your domain:
1. Go to Site settings → Domain management
2. Add custom domain
3. Follow Netlify's DNS instructions

## ✅ Checklist Before Deploy

- [ ] Update copyright year in footer if needed
- [ ] Add hero image (optional but recommended)
- [ ] Test form submission after deployment
- [ ] Verify all links work
- [ ] Check mobile responsiveness

## 📱 Testing

After deployment, test:
- Form submission
- Mobile view
- All anchor links
- Page load speed

---

**Site Stack:**
- Pure HTML/CSS (no build step needed)
- Netlify Forms (built-in)
- Google Fonts (Inter & Oswald)
- Mobile-first responsive design