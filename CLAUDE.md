# Claude Memory - Souptoys.com Project

## Project Overview
This is the Souptoys.com website - an interactive toy engine landing page with modern design and optimized performance.

## Repository Information
- **GitHub Repository**: https://github.com/mixedmediaservice/souptoyscom
- **Domain**: souptoys.com
- **Hosting**: Vercel (configured)

## Recent Work Completed

### 1. Initial Setup & GitHub Integration
- Initialized git repository
- Pushed project to GitHub: https://github.com/mixedmediaservice/souptoyscom
- Created initial commit with all project files

### 2. WebP Image Optimization (Latest Work)
**Completed**: Comprehensive image optimization for better performance
- Converted all images to WebP format using Python Pillow
- Achieved significant file size reductions:
  - `background.jpg`: 50.5% reduction (220KB → 109KB)
  - `background.png`: 75.6% reduction (344KB → 84KB)
  - `favicon-512x512.jpg`: 43.9% reduction (33KB → 19KB)
  - `pine-wood-texture.jpg`: 18.3% reduction (1MB → 863KB)
  - `preview.jpg`: 48.7% reduction (110KB → 56KB)
- Updated HTML to use `<picture>` elements with WebP and fallback images
- Updated CSS background to use WebP with JPG fallback
- Total project size reduced by ~27% overall

### 3. Vercel DNS Configuration
**DNS Settings Required** (User needs to implement):
- Remove Squarespace A records (198.185.159.144, 198.49.23.145)
- Remove custom IP (76.76.21.21)
- Add Vercel A records:
  - `@` A `76.76.21.241`
  - `@` A `76.223.126.88`
  - `@` A `108.156.12.38`
  - `@` A `76.223.126.90`
- Keep existing: `www CNAME cname.vercel-dns.com`, Mailgun MX records

## Current Project Structure
```
/
├── index.html (updated with WebP picture elements)
├── style.css (updated with WebP backgrounds + fallbacks)
└── assets/images/
    ├── background.jpg/.png/.webp (all formats available)
    ├── favicon-512x512.jpg/.webp
    ├── pine-wood-texture.jpg/.webp
    ├── preview.jpg/.webp
    └── favicon.ico
```

## Git Status
- **Current Branch**: main
- **Latest Commit**: "Optimize images with WebP format and update references"
- **Status**: 1 commit ahead of origin/main (ready to push if needed)

## Next Steps
1. User should update DNS settings in domain registrar for Vercel deployment
2. Consider pushing the latest WebP optimization commit: `git push`
3. Test website performance after WebP implementation
4. Monitor loading times and Core Web Vitals improvements

## Technical Notes
- All images now have WebP versions with fallbacks for browser compatibility
- CSS uses progressive enhancement (fallback → WebP)
- HTML uses `<picture>` elements for optimal image delivery
- Project is ready for production deployment on Vercel

## Tools Used
- Python Pillow for image conversion
- Git for version control
- WebP format for modern browsers with fallbacks for older browsers