# 📍 GPS Pro - Samsung Galaxy S23 Ultra Edition

Professional GPS surveying tool optimized for Samsung Galaxy S23 Ultra's dual-band GPS (L1+L5).

## Features

- ✅ Real-time GPS tracking with high accuracy
- ✅ Dual-band GPS support (L1+L5) for Samsung S23 Ultra
- ✅ Point A & B capture with coordinates
- ✅ Distance calculation using Haversine formula
- ✅ Elevation and slope measurements
- ✅ Signal quality indicator
- ✅ Wake Lock API support (keep screen active)
- ✅ Modern dark UI with animations
- ✅ Haptic feedback (vibration)
- ✅ Progressive Web App ready

## 🚀 Deploy to Netlify

### Option 1: Drag & Drop (Easiest)
1. Go to [netlify.com](https://netlify.com) and sign up/login
2. Click "Add new site" → "Deploy manually"
3. Drag the entire folder into the upload zone
4. Your app will be live at `https://[random-name].netlify.app`

### Option 2: Netlify CLI
```bash
npm install -g netlify-cli
netlify deploy --prod
```

### Option 3: Git Deploy
1. Push files to GitHub repository
2. Connect repository to Netlify
3. Deploy automatically

## 📱 Requirements

- HTTPS connection (required for Geolocation API)
- Browser with GPS/location support
- Location permissions enabled
- Works best on Samsung Galaxy S23 Ultra

## 🔒 Security

The app includes:
- HTTPS enforcement via `netlify.toml`
- Security headers (X-Frame-Options, CSP, etc.)
- Geolocation permission policy
- No external dependencies

## 📖 Usage

1. **Open the app** on your mobile device via HTTPS
2. **Grant location permission** when prompted
3. **Press "Iniciar GPS"** to start tracking
4. **Wait for good signal** (< 10m accuracy recommended)
5. **Capture Point A** at first location
6. **Move to second location**
7. **Capture Point B** 
8. **View results** - distance, elevation, slope

## 🛠 Technical Details

- Single-page application (SPA)
- No build process required
- Pure HTML/CSS/JavaScript
- Uses Geolocation API with `enableHighAccuracy: true`
- Haversine formula for distance calculation
- Wake Lock API for screen management

## 📄 Files Included

- `index.html` - Main application
- `netlify.toml` - Netlify configuration (HTTPS redirect, headers)
- `README.md` - This file

## 🌐 Custom Domain (Optional)

After deploying to Netlify:
1. Go to Site settings → Domain management
2. Add your custom domain
3. Configure DNS records as instructed

## 📞 Support

For issues or questions about the app functionality, check:
- Browser console for errors
- Location permissions in device settings
- HTTPS is enabled
- Signal quality indicator

---

**Version:** 2.0  
**Optimized for:** Samsung Galaxy S23 Ultra  
**License:** MIT
