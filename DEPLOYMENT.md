# Deployment Guide - Elite Motors Website

This guide provides step-by-step instructions for deploying the Elite Motors car dealership website.

## 🚀 Quick Deployment Options

### Option 1: Vercel (Recommended)
1. Install Vercel CLI: `npm i -g vercel`
2. In project directory: `vercel`
3. Follow prompts to deploy
4. Your site will be live at a vercel.app URL

### Option 2: Netlify
1. Build the project: `pnpm run build`
2. Drag and drop the `dist/` folder to netlify.com/drop
3. Your site will be live instantly

### Option 3: GitHub Pages
1. Push code to GitHub repository
2. Go to repository Settings > Pages
3. Select source branch and folder
4. Enable GitHub Actions for automatic builds

## 🔧 Manual Deployment

### Step 1: Build the Project
```bash
cd car-dealership
pnpm install
pnpm run build
```

### Step 2: Upload Files
Upload the contents of the `dist/` folder to your web server.

### Step 3: Configure Server
Ensure your server serves `index.html` for all routes (SPA configuration).

#### Apache (.htaccess)
```apache
RewriteEngine On
RewriteCond %{REQUEST_FILENAME} !-f
RewriteCond %{REQUEST_FILENAME} !-d
RewriteRule . /index.html [L]
```

#### Nginx
```nginx
location / {
    try_files $uri $uri/ /index.html;
}
```

## 🌐 Domain Configuration

### Custom Domain Setup
1. Point your domain to your hosting provider
2. Configure DNS A records or CNAME
3. Enable HTTPS/SSL certificate
4. Test all functionality

### Environment Variables
No environment variables required for this static site.

## 📊 Performance Optimization

### Before Deployment
- Images are already optimized
- CSS is minified in build
- JavaScript is bundled and minified
- Unused code is tree-shaken

### Post-Deployment
- Enable gzip compression
- Set up CDN (CloudFlare, AWS CloudFront)
- Configure caching headers
- Monitor Core Web Vitals

## 🔍 Testing Checklist

Before going live, test:
- [ ] All navigation links work
- [ ] Search functionality
- [ ] Filter options
- [ ] Contact form submission
- [ ] Mobile responsiveness
- [ ] Page load speed
- [ ] Cross-browser compatibility

## 📱 Mobile Testing

Test on various devices:
- iPhone (Safari)
- Android (Chrome)
- iPad (Safari)
- Various screen sizes

## 🛠️ Maintenance

### Regular Updates
- Update dependencies monthly
- Monitor for security vulnerabilities
- Backup website files
- Update car inventory as needed

### Content Updates
- Add new vehicles to inventory
- Update company information
- Refresh testimonials
- Update contact information

## 🚨 Troubleshooting

### Common Issues

**Build Fails**
- Check Node.js version (v18+)
- Clear node_modules and reinstall
- Check for syntax errors

**Images Not Loading**
- Verify image paths in components
- Check image file formats (jpg, png, webp)
- Ensure images are in src/assets/cars/

**Styling Issues**
- Clear browser cache
- Check Tailwind CSS compilation
- Verify CSS imports

**Form Not Working**
- Check form validation
- Verify event handlers
- Test in different browsers

## 📞 Support

For deployment issues or questions:
1. Check this guide first
2. Review error messages
3. Test locally before deploying
4. Contact development team if needed

## 🔐 Security Considerations

- Enable HTTPS
- Set security headers
- Regular dependency updates
- Monitor for vulnerabilities
- Backup regularly

---

**Happy Deploying!** 🚀

