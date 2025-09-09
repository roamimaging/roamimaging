# Roam Imaging Utah Website

This repository contains the code for roamimagingutah.com - a mobile 3D/4D ultrasound service in Utah.

## About

Roam Imaging Utah provides mobile 2D/3D/4D (HD Live) elective ultrasounds across Weber, Davis & Salt Lake Counties. They offer gender reveal, early heartbeat, and keepsake scans in the comfort of your home.

## Technology Stack

- **Platform**: Built with Framer
- **Analytics**: Google Analytics (G-N39VVW8JJD)
- **Tag Management**: Google Tag Manager (GTM-TW856PN5)
- **Fonts**: Inter, DM Sans, Poppins (via Google Fonts)

## Project Structure

```
roamimagingutah.com/
├── index.html              # Main HTML file
├── assets/
│   ├── fonts/             # Font files (woff2)
│   ├── images/            # Images and graphics
│   └── js/                # JavaScript files
├── download_assets.sh      # Asset download script
├── download_clean_assets.sh # Clean asset download script
└── README.md              # This file
```

## Getting Started

1. Clone this repository
2. Open `index.html` in a web browser to view locally
3. For development, consider using a local server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve
   ```

## Deployment

The website is currently hosted on Framer. To deploy changes:

1. Make your modifications
2. Commit changes to Git
3. Push to your GitHub repository
4. Deploy via your preferred hosting service

## Assets

- Fonts are loaded from Google Fonts and Framer's CDN
- Images are served from Framer's CDN (framerusercontent.com)
- All essential assets have been downloaded locally for backup

## SEO & Analytics

- Google Analytics tracking implemented
- Open Graph and Twitter meta tags configured
- Mobile-responsive design
- Optimized for search engines

## Development

To make changes to the website:

1. Edit `index.html` for content changes
2. Update asset files in the `assets/` directory
3. Test locally before deployment
4. Commit and push changes

## Support

For questions about the website code, please create an issue in this repository.