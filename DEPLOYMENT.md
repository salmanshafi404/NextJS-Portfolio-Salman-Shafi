# Deployment Guide for Salman Shafi Portfolio

This guide provides step-by-step instructions for deploying your optimized portfolio website to Vercel.

## 🚀 Quick Deployment to Vercel

### 1. Prerequisites
- GitHub account with your repository
- Vercel account (free tier available)
- Node.js 18+ installed locally

### 2. Environment Variables
Before deploying, make sure to set these environment variables in Vercel:

```bash
# SMTP Configuration for AWS SES
# Replace with your actual AWS SES credentials
SMTP_HOST=email-smtp.ap-southeast-1.amazonaws.com
SMTP_USERNAME=your-aws-ses-username
SMTP_PASSWORD=your-aws-ses-password
SMTP_PORT=587
SMTP_SECURE=false

# Email Configuration
# Update with your actual email addresses
FROM_EMAIL_NAME=Your Name Contact
FROM_EMAIL=no-reply@yourdomain.com
TO_EMAIL=your-email@gmail.com

# Application Configuration
# Update with your actual domain
NEXT_PUBLIC_SITE_URL=https://yourdomain.com
```

**Note:** Copy `.env.example` to `.env.local` and fill in your actual values for local development.

### 3. Deployment Steps

#### Option A: Vercel CLI (Recommended)
```bash
# Install Vercel CLI
npm i -g vercel

# Login to Vercel
vercel login

# Deploy
vercel --prod
```

#### Option B: GitHub Integration
1. Go to [vercel.com](https://vercel.com)
2. Click "New Project"
3. Import your GitHub repository
4. Add environment variables in Project Settings
5. Deploy

### 4. Domain Configuration
1. In Vercel Dashboard → Project Settings → Domains
2. Add your custom domain: `salmanshafi.net`
3. Configure DNS records as instructed by Vercel

## 🔧 Performance Optimizations Applied

### Build Optimizations
- ✅ **Image Optimization**: WebP/AVIF formats with Next.js Image component
- ✅ **Code Splitting**: Automatic chunking for optimal loading
- ✅ **Tree Shaking**: Removed unused code
- ✅ **Minification**: CSS/JS compression enabled
- ✅ **Console Removal**: Production builds remove console.log statements

### SEO Optimizations
- ✅ **Meta Tags**: Complete OpenGraph and Twitter Cards
- ✅ **Structured Data**: JSON-LD schema for rich snippets
- ✅ **Sitemap**: Dynamic sitemap generation
- ✅ **Robots.txt**: Proper crawling instructions
- ✅ **Canonical URLs**: Prevent duplicate content issues

### Security Headers
- ✅ **XSS Protection**: Cross-site scripting prevention
- ✅ **Content Security**: Prevents content injection
- ✅ **Frame Options**: Clickjacking protection
- ✅ **MIME Sniffing**: Content type validation

### Performance Features
- ✅ **Contact Form**: Working email with premium styling
- ✅ **Responsive Design**: Mobile-first approach
- ✅ **Loading States**: Smooth user experience
- ✅ **Error Handling**: Graceful error management

## 📊 Build Statistics

```
Route (app)                                 Size  First Load JS
├ ○ /_not-found                            991 B         101 kB
├ ƒ /api/contact                           127 B        99.8 kB
└ ○ /sitemap.xml                           127 B        99.8 kB
+ First Load JS shared by all            99.7 kB
```

## 🔍 Testing Checklist

Before deploying, verify:
- [ ] `npm run build` completes successfully
- [ ] `npm run start` serves the production build
- [ ] Contact form sends emails correctly
- [ ] All images load properly
- [ ] Mobile responsiveness works
- [ ] SEO meta tags are present
- [ ] Sitemap is accessible at `/sitemap.xml`
- [ ] Robots.txt is accessible at `/robots.txt`

## 🌐 Post-Deployment Validation

### 1. Performance Testing
- Use [PageSpeed Insights](https://pagespeed.web.dev/)
- Check [GTmetrix](https://gtmetrix.com/) scores
- Verify Core Web Vitals

### 2. SEO Validation
- Test with [Rich Results Test](https://search.google.com/test/rich-results)
- Submit sitemap to Google Search Console
- Verify OpenGraph with [Facebook Debugger](https://developers.facebook.com/tools/debug/)

### 3. Security Testing
- Check headers with [Security Headers](https://securityheaders.com/)
- Verify SSL certificate
- Test contact form functionality

## 🔧 Troubleshooting

### Common Issues
1. **Build Fails**: Check environment variables are set
2. **Images Not Loading**: Verify image paths and formats
3. **Contact Form Not Working**: Check SMTP credentials
4. **Slow Loading**: Enable compression and check bundle size

### Support Resources
- [Vercel Documentation](https://vercel.com/docs)
- [Next.js Documentation](https://nextjs.org/docs)
- [Portfolio Repository Issues](https://github.com/your-repo/issues)

## 📈 Performance Monitoring

Set up monitoring with:
- Vercel Analytics (built-in)
- Google Analytics 4
- Vercel Speed Insights
- Real User Monitoring (RUM)

---

**Ready to deploy?** Your portfolio is now optimized for production with all modern best practices implemented! 