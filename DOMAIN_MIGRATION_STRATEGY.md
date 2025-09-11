# Domain Migration Strategy: GitHub Pages → roamimagingutah.com

## Overview
This document outlines the complete strategy for migrating from GitHub Pages (roamimaging.github.io/roamimaging) to the primary domain (roamimagingutah.com) to maximize SEO impact and business growth.

## Current Status Assessment

### ✅ What's Ready for Migration
- **Technical SEO Foundation**: robots.txt, sitemap.xml, structured data
- **Content Structure**: 9 optimized pages with comprehensive SEO
- **County-Specific Landing Pages**: Weber, Davis, Salt Lake targeting
- **Service-Specific Pages**: Early pregnancy, gender reveal, 3D/4D
- **Blog Foundation**: Content hub for long-tail keyword targeting
- **Internal Linking Strategy**: Cross-page SEO architecture

### 📊 Current GitHub Pages Performance
```
Pages Created: 9 total
- index.html (main homepage)
- weber-county-mobile-ultrasound.html
- davis-county-mobile-ultrasound.html  
- salt-lake-county-mobile-ultrasound.html
- gender-reveal-ultrasound-utah.html
- early-pregnancy-ultrasound-utah.html
- 3d-4d-ultrasound-at-home-utah.html
- blog.html
- robots.txt, sitemap.xml
```

## Migration Timeline & Strategy

### Phase 1: Pre-Migration Preparation (Week 1)
**Goal**: Ensure seamless transition with zero SEO loss

#### Technical Preparation
1. **Domain Setup**
   - Configure roamimagingutah.com DNS settings
   - Set up hosting environment (recommend Netlify/Vercel for static sites)
   - SSL certificate installation

2. **Content Audit & Updates**
   - Update all internal links from GitHub Pages URLs to new domain
   - Verify all asset URLs (images, videos) are working
   - Test mobile responsiveness across all pages

3. **SEO Preparation**
   - Update sitemap.xml with new domain URLs
   - Update structured data with new domain references
   - Prepare 301 redirect mapping

#### Pre-Migration Checklist
```
□ Domain DNS configured
□ SSL certificate installed
□ All internal links updated to new domain
□ Asset URLs verified and working
□ sitemap.xml updated
□ Structured data updated
□ Google Analytics/Tag Manager updated
□ 301 redirect plan created
```

### Phase 2: Migration Execution (Week 2)
**Goal**: Execute migration with proper redirects and monitoring

#### Migration Steps
1. **Deploy to New Domain**
   - Upload all files to roamimagingutah.com hosting
   - Test all pages and functionality
   - Verify Google Tag Manager tracking

2. **Implement 301 Redirects**
   ```
   GitHub Pages → New Domain Redirects:
   roamimaging.github.io/roamimaging/ → roamimagingutah.com/
   roamimaging.github.io/roamimaging/weber-county-mobile-ultrasound.html → roamimagingutah.com/weber-county-mobile-ultrasound
   [Continue for all pages...]
   ```

3. **Search Engine Updates**
   - Submit new sitemap to Google Search Console
   - Update Google My Business profile with new website
   - Request reindexing of priority pages

#### Migration Day Checklist
```
□ All files deployed to new domain
□ 301 redirects implemented and tested
□ New sitemap submitted to Google Search Console
□ Google Analytics tracking verified
□ Google My Business updated
□ All pages loading correctly
□ Mobile responsiveness confirmed
```

### Phase 3: Post-Migration Monitoring (Weeks 3-4)
**Goal**: Monitor performance and optimize based on data

#### Monitoring Tasks
1. **SEO Performance Tracking**
   - Monitor Google Search Console for crawl errors
   - Track keyword rankings for target terms
   - Monitor organic traffic levels

2. **Technical Monitoring**
   - Check page load speeds
   - Monitor for broken links or 404 errors
   - Verify all forms and CTAs working

3. **Analytics Setup**
   - Compare traffic before/after migration
   - Set up conversion tracking for phone calls and form submissions
   - Monitor bounce rates and user engagement

## SEO Impact Projections

### Short-Term Impact (0-3 months)
- **Expected traffic dip**: 10-20% during first 2-4 weeks (normal for migrations)
- **Recovery timeline**: 4-6 weeks to pre-migration levels
- **Authority transfer**: 301 redirects preserve 85-90% of existing authority

### Medium-Term Growth (3-6 months)
- **Primary domain authority boost**: +25-35% SEO strength
- **Local search improvements**: Better rankings for "ultrasound Utah" terms
- **Brand recognition**: Improved click-through rates with branded domain

### Long-Term Projections (6-12 months)
- **Revenue growth target**: $3,000 → $12,000 monthly (4x growth)
- **Keyword ranking improvements**: Top 3 positions for 15+ target keywords
- **Local dominance**: #1 rankings for county-specific searches

## Domain Benefits Analysis

### ✅ Advantages of roamimagingutah.com
1. **Brand Authority**: Professional domain builds trust
2. **Local SEO**: "Utah" in domain helps geographic targeting
3. **Memorability**: Easier for customers to remember and type
4. **Email Marketing**: Professional email addresses (@roamimagingutah.com)
5. **Marketing Materials**: Clean URLs for print/digital advertising

### 📈 Expected SEO Improvements
```
Current GitHub Pages Authority: ~15-20/100
Expected roamimagingutah.com Authority: 35-45/100

Keyword Ranking Improvements:
- "mobile ultrasound utah" → Top 3 (currently ~15)
- "3d 4d ultrasound utah" → Top 5 (currently ~25)  
- "gender reveal ultrasound utah" → #1 (currently ~10)
- "ultrasound at home utah" → Top 3 (currently ~20)
```

## Technical Implementation Guide

### DNS Configuration
```
A Record: @ → [Hosting IP]
CNAME: www → roamimagingutah.com
```

### 301 Redirect Rules (.htaccess)
```apache
RewriteEngine On
RewriteRule ^weber-county-mobile-ultrasound.html$ /weber-county-mobile-ultrasound [R=301,L]
RewriteRule ^davis-county-mobile-ultrasound.html$ /davis-county-mobile-ultrasound [R=301,L]
RewriteRule ^salt-lake-county-mobile-ultrasound.html$ /salt-lake-county-mobile-ultrasound [R=301,L]
RewriteRule ^gender-reveal-ultrasound-utah.html$ /gender-reveal-ultrasound-utah [R=301,L]
RewriteRule ^early-pregnancy-ultrasound-utah.html$ /early-pregnancy-ultrasound-utah [R=301,L]
RewriteRule ^3d-4d-ultrasound-at-home-utah.html$ /3d-4d-ultrasound-at-home-utah [R=301,L]
RewriteRule ^blog.html$ /blog [R=301,L]
```

### Google Search Console Setup
1. Add roamimagingutah.com as new property
2. Verify ownership via DNS or HTML file
3. Submit updated sitemap.xml
4. Set up URL inspection for priority pages

## Risk Mitigation

### Potential Issues & Solutions
1. **Temporary Traffic Drop**
   - *Solution*: Proper 301 redirects + patient monitoring
   - *Timeline*: 4-6 week recovery expected

2. **Broken Internal Links**
   - *Solution*: Comprehensive link audit before migration
   - *Backup*: Keep GitHub Pages live for 30 days as fallback

3. **Analytics Data Loss**
   - *Solution*: Update Google Analytics before migration
   - *Backup*: Historical data preservation in separate view

## Success Metrics

### Week 1-2 Targets
- ✅ Zero 404 errors on new domain
- ✅ All pages indexed by Google
- ✅ Google Tag Manager tracking functional

### Month 1 Targets
- 📈 Recover 85%+ of pre-migration organic traffic
- 🎯 Maintain top 10 rankings for primary keywords
- 📞 Phone call conversion rate maintained/improved

### Month 3 Targets
- 🚀 Exceed pre-migration traffic by 25%
- 🏆 Achieve top 5 rankings for 10+ target keywords
- 💰 Revenue growth to $6,000+ monthly

### Month 6 Targets
- 📊 4x traffic growth vs. pre-migration baseline
- 🎯 #1 rankings for "mobile ultrasound [county]" terms
- 💼 $12,000+ monthly revenue target achieved

## Post-Migration Optimization

### Content Expansion Plan
1. **Blog Content Calendar**: 2 posts/week targeting long-tail keywords
2. **Service Page Updates**: Add customer testimonials and case studies
3. **FAQ Expansions**: Target voice search and mobile queries
4. **Local Landing Pages**: Add city-specific pages within counties

### Advanced SEO Tactics
1. **Schema Markup Expansion**: Add FAQ, Review, and Service schemas
2. **Local Citations**: Build listings on Utah-specific directories
3. **Link Building**: Partner with Utah pregnancy/parenting websites
4. **Google My Business**: Optimize for local search dominance

## Conclusion

The migration to roamimagingutah.com represents a critical opportunity to:
- **Establish domain authority** in the competitive Utah ultrasound market
- **Improve local SEO performance** with geographic domain signals
- **Build long-term brand recognition** and customer trust
- **Scale revenue from $3K to $12K monthly** through improved search visibility

**Recommended Migration Date**: Within 2-4 weeks of completing Phase 2 content creation

**Expected ROI**: 300-400% revenue increase within 6 months of migration

**Key Success Factor**: Proper execution of 301 redirects and comprehensive post-migration monitoring