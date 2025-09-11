# Roam Imaging Utah - Framer Style Guide

## Overview
This style guide ensures all pages maintain exact visual consistency with the main roamimagingutah.com site deployed at https://roamimaging.github.io/roamimaging/.

## Color Palette (CSS Variables)
```css
/* Primary Brand Colors */
--token-3d4ba2c0-7533-48b2-baab-5128ed0b341d: rgb(255, 255, 255);    /* Primary White */
--token-c36e0eff-22d5-44da-941a-7a289e1e37b5: rgb(34, 34, 34);       /* Primary Dark */
--token-66a971ed-c926-4486-8ccd-05f35df408ec: rgb(57, 115, 225);     /* Brand Blue */
--token-56f172c9-0cf1-4a02-8b5e-0f5042f48b12: rgb(244, 244, 244);    /* Light Gray */
--token-0985a85b-39fd-4d8e-9378-5ec3a2695313: rgb(234, 192, 222);    /* Pink Accent */
--token-cdf2787f-a2da-4c79-85f4-35a9d1de9817: rgb(13, 13, 13);       /* Black */
--token-10ddab5c-c24d-401b-a44f-43a54324b6d5: rgba(255, 255, 255, .05); /* White Overlay */
--token-75bfb065-ffeb-4303-a244-a27fb0df944c: rgb(13, 13, 13);       /* Dark Alt */
--token-2130aa8d-3357-4201-89df-bed70daf06c2: rgba(19, 19, 20, .3);  /* Dark Overlay */

/* Usage Map */
Primary White: rgb(255, 255, 255)
Primary Dark: rgb(34, 34, 34)
Brand Blue: rgb(57, 115, 225)
Light Gray: rgb(244, 244, 244)
Card Background: rgb(248, 249, 250)
```

## Typography System

### Font Stack (Priority Order)
1. **Primary:** Inter (Framer CDN + Google Fonts backup)
2. **Secondary:** DM Sans (Multiple weights: 400, 500, 700, 900)
3. **Accent:** Poppins (Primary for headlines)
4. **Monospace:** Fragment Mono (Special usage)

### Font Weight Hierarchy
```css
/* Standard Weights */
font-weight: 400; /* Normal text */
font-weight: 500; /* Medium emphasis */
font-weight: 700; /* Bold headings */
font-weight: 900; /* Extra bold (DM Sans only) */
```

### Typography Scale
```css
/* Hero Headlines (H1) */
font-family: "Poppins", sans-serif;
font-weight: 700;
font-size: 67-82px (desktop), 13px (mobile via CSS variables);
line-height: 70-80px;
color: rgb(255, 255, 255);
text-align: center;
font-style: italic (for certain headers);

/* Section Headlines (H2) */
font-family: "Poppins", sans-serif;
font-weight: 700;
font-size: 2.5rem;
color: rgb(34, 34, 34);
margin-bottom: 30px;

/* Service Card Headlines (H3) */
font-family: "Poppins", sans-serif;
font-weight: 600;
font-size: 1.5rem;
color: rgb(34, 34, 34);
margin-bottom: 15px;

/* Body Text */
font-family: "Inter", sans-serif;
font-size: 1.1-1.2rem;
color: rgb(34, 34, 34);
line-height: 1.6;

/* Service Pricing */
font-family: "Inter", sans-serif;
font-weight: 600;
color: rgb(57, 115, 225);
```

## Layout System

### Framer Breakpoint System
```css
/* Desktop Large (1728px+) */
@media(min-width: 1728px) { 
  .hidden-72rtr7 { display: none !important; }
}

/* Desktop/Tablet (900px - 1727px) */
@media(min-width: 900px) and (max-width: 1727.98px) { 
  .hidden-1qe4lli { display: none !important; }
}

/* Mobile (0 - 899px) */
@media(max-width: 899.98px) { 
  .hidden-n62rfh { display: none !important; }
}
```

### Container Structure
```css
/* Main Content Container */
max-width: 1200px;
margin: 0 auto;
padding: 60px 20px;

/* Grid Layouts */
display: grid;
grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
gap: 30px;

/* Service Cards Grid */
grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
gap: 20px;
```

## Component Library

### Hero Video Section
```html
<div class="framer-14o57qh">
  <div class="framer-1hazkug-container">
    <div class="ssr-variant hidden-n62rfh hidden-1qe4lli">
      <video src="https://framerusercontent.com/assets/2FOxVRZ7SbKzHofdThZDJXjeglQ.mp4" 
             loop poster="https://framerusercontent.com/images/AAFu8GasR4F0ja0RwcGrbpQW7A.png" 
             muted playsinline 
             style="width:100%;height:100%;border-radius:24px;object-fit:cover;">
      </video>
    </div>
  </div>
</div>
```

### Responsive Headers
```html
<!-- Mobile Header -->
<svg class="framer-1fdodpc hidden-72rtr7 hidden-1qe4lli" viewBox="0 0 318 60">
  <foreignObject width="100%" height="100%">
    <h1 style="--framer-font-family:'Poppins', sans-serif;
               --framer-font-size:13.04646158506732px;
               --framer-font-style:italic;
               --framer-line-height:30px;
               --framer-text-color:rgb(255, 255, 255);">
      [County] Mobile Ultrasound<br/>#1 3D 4D Home Ultrasound [City] Utah
    </h1>
  </foreignObject>
</svg>

<!-- Desktop Header -->
<svg class="framer-12aeoau hidden-n62rfh" viewBox="0 0 1041 70">
  <foreignObject width="100%" height="100%">
    <h1 style="--framer-font-size:23.511531923013333px;
               --framer-line-height:70px;">
      [County] Mobile Ultrasound - 3D 4D Home Ultrasound [Cities]
    </h1>
  </foreignObject>
</svg>
```

### Service Cards
```css
/* Card Container */
background: rgb(248, 249, 250);
padding: 30px;
border-radius: 20px;
text-align: center;
box-shadow: none; /* Framer uses subtle shadows */

/* City Cards */
background: white;
padding: 20px;
border-radius: 15px;
box-shadow: 0 4px 15px rgba(0,0,0,0.1);
```

### Buttons
```css
/* Primary CTA Button */
display: inline-block;
background: rgb(57, 115, 225);
color: white;
padding: 15px 30px;
border-radius: 50px;
font-family: "Inter", sans-serif;
font-weight: 600;
font-size: 1.1rem;
text-decoration: none;
transition: transform 0.3s ease;

/* Hero Button (White) */
background: rgb(255, 255, 255);
color: rgb(34, 34, 34);
border-radius: 50px;
border: 0px solid rgb(255, 255, 255);
```

## Required Page Structure

### HTML Document Structure
```html
<!doctype html>
<!-- ✨ Built with Framer • https://www.framer.com/ -->
<html lang="en">
<head>
  <!-- Google Tag Manager -->
  <!-- Framer Meta Tags -->
  <meta name="generator" content="Framer b9489e0">
  <meta name="framer-search-index" content="https://framerusercontent.com/sites/WjP1ysmiVJtDkh4Ba8KS8/searchIndex-fNLNgJ7vf93G.json">
  
  <!-- SEO Meta Tags -->
  <!-- LocalBusiness Schema -->
  <!-- Font Declarations -->
  <!-- Framer CSS -->
</head>
<body style="margin:0;padding:0;box-sizing:border-box">
  <!-- Framer Container -->
  <div id="main" data-framer-hydrate-v2="[FRAMER_DATA]">
    <div data-framer-root class="framer-dl27v framer-8h6LU framer-4X5oD framer-72rtr7">
      <!-- Content -->
    </div>
  </div>
</body>
</html>
```

### Required Framer CSS Classes
```css
/* Core Framer Classes (Must Include) */
.framer-dl27v    /* Root container */
.framer-8h6LU    /* Layout wrapper */
.framer-4X5oD    /* Content wrapper */
.framer-72rtr7   /* Responsive wrapper */

/* Component Classes */
.framer-14o57qh  /* Hero video section */
.framer-1hazkug-container /* Video container */
.framer-1nct5n8  /* Header content */
.framer-1fdodpc  /* Mobile header */
.framer-12aeoau  /* Desktop header */
.framer-1lyigs4  /* Hero title */

/* Utility Classes */
.ssr-variant     /* Server-side rendering */
.hidden-72rtr7   /* Hide on desktop large */
.hidden-1qe4lli  /* Hide on tablet/desktop */
.hidden-n62rfh   /* Hide on mobile */
```

## Content Guidelines

### Service Pricing (Consistent)
- **Early Pregnancy Ultrasound:** $89.99 (7-14 weeks)
- **Gender Reveal Ultrasound:** $125.99 (16+ weeks)
- **3D/4D "Meet Your Baby" Session:** $185.99 (20-32 weeks)

### Geographic Targeting
- **Weber County:** Ogden, Roy, Clearfield, Layton, North Ogden, South Ogden
- **Davis County:** Bountiful, Farmington, Kaysville, Layton, Centerville, Woods Cross
- **Salt Lake County:** Salt Lake City, West Valley City, Murray, Sandy, South Jordan, West Jordan

### SEO Requirements
1. **Structured Data:** LocalBusiness schema with geographic coordinates
2. **Meta Tags:** County-specific titles and descriptions
3. **Internal Linking:** Cross-reference between county pages
4. **Image Optimization:** Use Framer CDN URLs
5. **Mobile Optimization:** Framer responsive breakpoints

## Asset URLs
```
Hero Video: https://framerusercontent.com/assets/2FOxVRZ7SbKzHofdThZDJXjeglQ.mp4
Video Poster: https://framerusercontent.com/images/AAFu8GasR4F0ja0RwcGrbpQW7A.png
Logo: https://framerusercontent.com/images/k26tCCUsc29iXU21E5iVZhP90.png
Main Image: https://framerusercontent.com/assets/dKJl8rFZEdFzXqKnktQKrvc3h74.jpg
Favicon: https://framerusercontent.com/images/ZQQiNKkCGZHYVxDRjkkmOSkqODI.png
```

## Quality Checklist
- [ ] All Framer CSS classes and data attributes preserved
- [ ] Responsive breakpoints (.hidden-* classes) implemented
- [ ] Font loading via Framer CDN + Google Fonts backup
- [ ] Video background displays correctly
- [ ] County-specific content and schema
- [ ] Cross-linking navigation functional
- [ ] Mobile-first responsive design
- [ ] Google Tag Manager implementation
- [ ] Brand color consistency maintained
- [ ] Typography hierarchy followed

## Implementation Notes
1. **Always use Framer CDN fonts first**, with Google Fonts as backup
2. **Preserve all data-framer-* attributes** for proper rendering
3. **Include full Framer hydration data** in main container
4. **Use exact CSS variable names** from token system
5. **Maintain SVG viewBox dimensions** for responsive headers
6. **Include proper schema markup** for local SEO