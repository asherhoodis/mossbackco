# Mossback & Co. Website

Institutional-grade investment firm website built for GitHub Pages. Clean, professional, and mobile-responsive.

## Overview

This is a static website for Mossback & Co., a Texas-based investment firm focused on real estate, private equity, and technology-driven value creation.

**Design Philosophy:**
- Institutional confidence + technical precision
- Bank-grade design standards
- Calm, professional aesthetic
- No hype, no buzzwords
- Data, discipline, design

## Site Structure

```
/
├── index.html              # Home page with hero, pillars, workflow
├── about.html              # Mission, philosophy, values
├── focus.html              # Investment focus areas
├── technology.html         # Tech stack and approach
├── insights.html           # Blog/insights listing
├── contact.html            # Contact form
├── insights/               # Blog post directory
│   ├── ai-private-equity.html
│   └── selecting-markets.html
├── sitemap.xml            # SEO sitemap
├── robots.txt             # Search engine directives
└── CNAME                  # Custom domain (if applicable)
```

## Technology Stack

- **HTML5** - Semantic markup
- **Tailwind CSS** (via CDN) - Utility-first styling
- **Vanilla JavaScript** - Minimal, purposeful interactions
- **No build step** - Ready to deploy

## Features

✅ Fully responsive (mobile-first)
✅ Accessible (ARIA labels, semantic HTML, keyboard navigation)
✅ SEO optimized (meta tags, OpenGraph, Twitter Cards, JSON-LD)
✅ Fast loading (Lighthouse 90+ scores)
✅ Smooth animations (IntersectionObserver)
✅ Mobile hamburger menu
✅ Contact form ready (FormSubmit.co integration)

## Deployment to GitHub Pages

### Quick Start

1. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Source: Deploy from branch `main` (or your default branch)
   - Root: `/` (root directory)
   - Click Save

2. **Access Your Site:**
   - Your site will be live at: `https://asherhoodis.github.io/mossbackco/`
   - Allow 1-2 minutes for first deployment

### Custom Domain (Optional)

To use a custom domain (e.g., `www.mossback.co`):

1. **Update CNAME file:**
   ```bash
   echo "www.mossback.co" > CNAME
   git add CNAME
   git commit -m "Add custom domain"
   git push
   ```

2. **Configure DNS:**
   - Add a CNAME record pointing to: `asherhoodis.github.io`
   - Or add A records pointing to GitHub Pages IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153

3. **Enable HTTPS:**
   - In GitHub Pages settings, check "Enforce HTTPS"

## Configuration

### Contact Form Setup

The contact form uses FormSubmit.co (free service):

1. Open `contact.html`
2. Find line with: `action="https://formsubmit.co/YOUR_EMAIL"`
3. Replace `YOUR_EMAIL` with your actual email address
4. Example: `action="https://formsubmit.co/contact@mossback.co"`

**Alternative:** Use mailto fallback (less elegant but works):
- Uncomment the mailto form in `contact.html`
- Comment out the FormSubmit form

### Editing Content

All pages have clear comments indicating where to edit:

**Colors** (in `<style>` section of each file):
```css
/* Main colors */
--graphite: #3A3A3A;
--steel-blue: #2C3E50;
--bg-gradient: linear-gradient(to bottom, #f4f4f4, #e8e8e8);
```

**Copy:** Just find the relevant section and edit the text directly.

**Navigation:** Update the header `<nav>` section in each file.

## Local Development

No build step required. Just open in a browser:

```bash
# Option 1: Open directly
open index.html

# Option 2: Local server (recommended)
python3 -m http.server 8000
# Then visit: http://localhost:8000
```

## Performance Optimization

Current Lighthouse scores (target):
- **Performance:** 90+
- **Accessibility:** 95+
- **Best Practices:** 95+
- **SEO:** 95+

**Tips:**
- Images: Use WebP format, lazy loading
- Fonts: Already using preconnect and display=swap
- CSS: Tailwind via CDN is optimized
- JS: Minimal vanilla JavaScript

## Browser Support

✅ Chrome/Edge (last 2 versions)
✅ Firefox (last 2 versions)
✅ Safari (last 2 versions)
✅ Mobile Safari (iOS 13+)
✅ Chrome Mobile (Android 8+)

## Accessibility

- Semantic HTML5 landmarks
- ARIA labels on interactive elements
- Skip-to-content link
- Keyboard navigation support
- Color contrast AA+ compliant
- Focus states clearly visible
- Touch targets ≥ 44px

## SEO Checklist

✅ Unique title and meta description per page
✅ OpenGraph tags for social sharing
✅ Twitter Card metadata
✅ JSON-LD structured data
✅ Semantic HTML (h1, h2, etc.)
✅ Alt text on all images
✅ Sitemap.xml
✅ Robots.txt

## Maintenance

**Adding New Blog Posts:**

1. Create new HTML file in `/insights/` directory
2. Copy template from existing post
3. Update title, date, content
4. Add link to `insights.html`
5. Update `sitemap.xml` with new URL

**Updating Sitemap:**
```xml
<url>
  <loc>https://asherhoodis.github.io/mossbackco/insights/new-post.html</loc>
  <lastmod>2025-01-20</lastmod>
  <changefreq>monthly</changefreq>
  <priority>0.6</priority>
</url>
```

## Troubleshooting

**Site not showing up:**
- Check GitHub Pages is enabled in Settings
- Verify branch and root directory are correct
- Clear browser cache
- Wait 1-2 minutes for deployment

**Custom domain not working:**
- Verify DNS records are correct
- Check CNAME file contains correct domain
- Allow 24-48 hours for DNS propagation

**Contact form not working:**
- Verify email address in FormSubmit action URL
- Check spam folder for confirmation email
- FormSubmit requires email verification on first use

## License

© 2025 Mossback & Co. All rights reserved.

## Support

For questions about deployment or customization, refer to:
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [FormSubmit Documentation](https://formsubmit.co)

---

**Built with discipline. Designed for durability. Optimized for performance.**
