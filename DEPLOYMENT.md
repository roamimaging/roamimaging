# Deployment Guide for Roam Imaging Utah Website

## GitHub Setup

### 1. Create GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click "New repository"
3. Name it `roamimagingutah-website`
4. Make it public (recommended for GitHub Pages)
5. Don't initialize with README (we already have one)

### 2. Connect Local Repository to GitHub

Your repository is already connected to: https://github.com/roamimaging/roamimaging.git

```bash
# The remote is already added. To push your changes:
git push -u origin main
```

**Note**: You'll need to authenticate with GitHub. Options:
- Use GitHub CLI: `gh auth login`
- Use personal access token
- Use SSH key authentication

### 3. Enable GitHub Pages (Free Hosting Option)

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll to "Pages" section
4. Under "Source", select "Deploy from a branch"
5. Select "main" branch and "/ (root)" folder
6. Click "Save"
7. Your site will be available at: `https://roamimaging.github.io/roamimaging/`

## Alternative Hosting Options

### Netlify (Recommended for Production)
1. Go to [Netlify.com](https://netlify.com)
2. Connect your GitHub account
3. Select your repository
4. Deploy settings:
   - Build command: Leave empty
   - Publish directory: `/`
5. Click "Deploy site"
6. Set up custom domain (roamimagingutah.com)

### Vercel
1. Go to [Vercel.com](https://vercel.com)
2. Import your GitHub repository
3. Deploy with default settings
4. Set up custom domain

### Traditional Web Hosting
1. Download all files from the repository
2. Upload to your web hosting via FTP/SFTP
3. Ensure `index.html` is in the root directory

## Making Updates with Claude Code

### Using Claude Code for Website Updates

1. **Clone the repository** (if working on a new machine):
   ```bash
   git clone https://github.com/roamimaging/roamimaging.git
   cd roamimaging
   ```

2. **Open Claude Code** in the project directory:
   ```bash
   claude-code .
   ```

3. **Make updates using Claude Code**:
   - "Update the contact information on the homepage"
   - "Add a new service to the services section"
   - "Improve the SEO meta tags"
   - "Update the pricing information"

4. **Deploy changes**:
   ```bash
   git add .
   git commit -m "Update: describe your changes"
   git push origin main
   ```

## Framer Migration Considerations

Since this website was originally built on Framer, some features may need attention:

### 1. Dynamic Content
- The original site may have had dynamic elements that are now static
- You may want to add form handling for contact forms
- Consider adding a CMS if content updates are frequent

### 2. Font Loading
- Fonts are loaded from both Google Fonts and Framer's CDN
- All essential fonts have been downloaded locally
- Update the HTML to use local fonts if needed for performance

### 3. Image Optimization
- Images are currently served from Framer's CDN
- Consider optimizing and hosting images locally for better performance
- Implement responsive images for different screen sizes

## SEO and Performance Improvements

### Using Claude Code for SEO
Ask Claude Code to help with:
- "Analyze the current SEO and suggest improvements"
- "Add structured data markup for local business"
- "Optimize images for better performance"
- "Add meta tags for social media sharing"

### Performance Optimization
- Compress images
- Minify CSS/JS (currently inline)
- Add caching headers
- Implement lazy loading for images

## Maintenance Tasks

### Regular Updates with Claude Code
- "Update business hours and contact information"
- "Add new testimonials to the website"
- "Update service pricing"
- "Improve mobile responsiveness"
- "Add new features like appointment booking"

### Analytics Setup
- Google Analytics is already configured (ID: G-N39VVW8JJD)
- Set up Google Search Console
- Monitor website performance and user behavior

## Backup Strategy

1. **GitHub as Primary Backup**: All code is version controlled
2. **Local Backups**: Keep local copies of important files
3. **Asset Backups**: All external assets have been downloaded locally

## Support

For technical issues with deployment or updates:
1. Check the repository's Issues tab
2. Use Claude Code for development assistance
3. Consult hosting provider documentation