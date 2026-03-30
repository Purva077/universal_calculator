# 🚀 Startup Guide — Universal Calculator Hub

Complete guide to launch your calculator app from zero to production.

## 📊 What You Have

- **96 calculators** across **18 categories**
- Full PWA with offline support
- Installable on all platforms
- Dark/Light theme
- Search, Favorites, History
- Mobile responsive

## 🎯 Quick Start (5 minutes)

### Option 1: GitHub Pages (Free, Recommended)

```bash
# 1. Create GitHub repo
# Go to github.com → New repository → "universal-calculator-hub"

# 2. Push code
cd calc-hub-app
git remote add origin https://github.com/YOUR_USERNAME/universal-calculator-hub.git
git branch -M main
git push -u origin main

# 3. Enable GitHub Pages
# Go to Settings → Pages → Source: GitHub Actions
# Your app auto-deploys on every push!

# 4. Live at:
# https://YOUR_USERNAME.github.io/universal-calculator-hub/
```

### Option 2: Netlify (Drag & Drop)

1. Go to [netlify.com](https://netlify.com)
2. Drag `calc-hub-app` folder onto deploy area
3. Done! Live in 30 seconds

### Option 3: Vercel

```bash
cd calc-hub-app
npx vercel
# Follow prompts → deployed!
```

### Option 4: Local Testing

```bash
cd calc-hub-app
npm start
# Opens at http://localhost:3000
```

## 📝 Before You Deploy

### 1. Update URLs

Replace `YOUR_USERNAME` in these files:
- `robots.txt` (line 4)
- `sitemap.xml` (all URLs)
- `package.json` (homepage, repository)
- `README.md` (clone URL, demo link)

### 2. Customize Branding (Optional)

**Change app name:**
- `manifest.json` → `name`, `short_name`
- `index.html` → `<title>`, meta tags
- `README.md` → heading

**Change colors:**
- `manifest.json` → `theme_color`, `background_color`
- `style.css` → `:root` CSS variables
- `index.html` → `<meta name="theme-color">`

**Change icons:**
- Replace `icons/icon-192.png` and `icons/icon-512.png`
- Or regenerate: open `generate-icons.html` in browser

### 3. Add Custom Domain (Optional)

**GitHub Pages:**
```bash
echo "yourcalc.com" > CNAME
git add CNAME
git commit -m "Add custom domain"
git push
```
Then add DNS records at your domain provider.

**Netlify/Vercel:**
Use their dashboard to add custom domain.

## 🔧 Configuration

### Service Worker Cache

Edit `sw.js` to change cache strategy:
```javascript
const CACHE = 'calchub-v2'; // Bump version to force update
```

### Add/Remove Calculators

1. Edit `app.js` → `CATS` object (add calculator definition)
2. Edit `app.js` → `FN` object (add calculator logic)
3. Edit `app.js` → `M` object in `buildUI()` (add UI template)
4. Test locally
5. Commit and push

See `CONTRIBUTING.md` for detailed guide.

## 📱 Testing PWA Install

### Android (Chrome)
1. Open your deployed URL
2. Tap menu → "Install app" or "Add to Home screen"
3. App installs like a native app

### iOS (Safari)
1. Open your deployed URL
2. Tap Share → "Add to Home Screen"
3. App appears on home screen

### Desktop (Chrome/Edge)
1. Open your deployed URL
2. Click install icon in address bar
3. App opens in standalone window

## 🎨 Customization Ideas

### Add More Calculators
- Crypto converters
- Cooking measurements
- Sports statistics
- Gaming calculators
- Regional tax calculators

### Add Features
- Export history to CSV
- Share results via URL
- Calculator presets/templates
- Multi-language support
- Voice input

### Monetization (Optional)
- Google AdSense (add script to `index.html`)
- Affiliate links in results
- Premium calculator pack
- Donation button

## 📈 Analytics (Optional)

Add Google Analytics to `index.html`:
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

## 🐛 Troubleshooting

**PWA not installing?**
- Check manifest.json is valid (use [Web Manifest Validator](https://manifest-validator.appspot.com/))
- Ensure HTTPS (required for PWA)
- Check browser console for errors

**Service Worker not updating?**
- Bump version in `sw.js`
- Hard refresh (Ctrl+Shift+R)
- Clear cache in DevTools

**Icons not showing?**
- Verify `icons/icon-192.png` and `icon-512.png` exist
- Check file sizes (should be ~3KB and ~10KB)
- Regenerate using `generate-icons.html`

## 📚 Resources

- [PWA Documentation](https://web.dev/progressive-web-apps/)
- [Service Worker Guide](https://developers.google.com/web/fundamentals/primers/service-workers)
- [Web App Manifest](https://developer.mozilla.org/en-US/docs/Web/Manifest)

## 🎉 You're Ready!

Your calculator app is production-ready. Deploy, share, and iterate based on user feedback.

Questions? Open an issue on GitHub.
