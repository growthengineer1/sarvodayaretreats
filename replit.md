# Sarvodaya Retreats Website

## Overview

Sarvodaya Retreats is a website for a backwater retreat sanctuary near Varkala, Kerala. The site serves artists, solo travelers, spiritual practitioners, and nature lovers by showcasing the intimate retreat space and enabling bookings/inquiries. The design is inspired by hand-drawn pencil art aesthetics with an organic, minimalist approach, taking visual cues from thenorth.in. The project emphasizes artistic presentation, philosophical depth, and a peaceful, authentic atmosphere.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture

**Technology Stack:**
- Pure HTML5, CSS3, and vanilla JavaScript (no frameworks)
- Static website with client-side rendering
- Responsive design for mobile-first approach

**Design System:**
- **Hand-drawn aesthetic**: SVG illustrations of organic elements (palm trees, yoga poses, water ripples, backwater landscapes, rescued animals)
- **Asymmetric layouts**: Organic, flowing grid structures rather than rigid frameworks
- **Typography hierarchy**: Serif fonts (Lora) for headlines and body text with generous letter spacing; sans-serif (Montserrat) for navigation and CTAs
- **Color palette**: CSS custom properties for consistent theming with sage green, warm cream, taupe, and charcoal tones

**Key Architectural Decisions:**
- **No JavaScript framework**: Chose vanilla JavaScript to maintain simplicity, fast load times, and minimize dependencies for a static, content-focused site
- **CSS Custom Properties**: Used for centralized color management and easy theme maintenance
- **Google Fonts integration**: External font loading for Lora (serif) and Montserrat (sans-serif) to achieve the artistic, sophisticated typography

**Layout Approach:**
- Smooth scrolling enabled for seamless navigation
- Mobile-responsive with flexible layouts
- Organic, asymmetrical grid system to match hand-drawn, artistic aesthetic
- Emphasis on visual breathing room and whitespace

### Content Architecture

**Primary Content Sections** (based on design brief):
- Hero/Landing section with backwater imagery
- About/Philosophy section explaining "Sarvodaya" (universal uplift)
- Facilities/Amenities showcasing retreat features
- Activities (swimming, yoga, meditation, nature immersion)
- Gallery with hand-drawn/illustrated elements
- Booking/Inquiry form or contact section
- Location details (3km from Varkala town center)

**Visual Elements:**
- Hand-drawn SVG illustrations as primary decorative elements
- Backwater landscape imagery
- Subtle rescued animal illustrations
- Meditation/yoga silhouettes
- Organic shapes and flowing water motifs

### Performance Considerations

**Optimization Strategy:**
- Static HTML/CSS/JS for maximum performance
- Minimal external dependencies (only Google Fonts)
- SVG graphics for scalable, lightweight illustrations
- Preconnect directives for font optimization
- Smooth scroll behavior without heavy JavaScript libraries

## External Dependencies

### Third-Party Services

**Google Fonts:**
- **Lora** (serif): 400, 500, 600 weights (regular and italic) for headlines and body text
- **Montserrat** (sans-serif): 300, 400, 500 weights for navigation and buttons
- Preconnect optimization enabled for faster font loading

**Potential Future Integrations** (not currently implemented):
- Booking system API or form submission service
- Email notification service for inquiries
- Image hosting CDN for gallery assets
- Analytics platform for visitor tracking
- Map integration for location display

### Browser APIs

- **Scroll behavior API**: For smooth scrolling navigation
- **Viewport meta tag**: For responsive mobile rendering
- Standard HTML5 semantic elements for SEO and accessibility

### Asset Dependencies

- SVG illustrations: Hand-drawn graphics for organic aesthetic (to be created/integrated)
- Image assets: Backwater photography, retreat facilities, nature scenes
- Icon sets: Potentially custom-drawn icons matching hand-drawn aesthetic

## Current Implementation Status (Updated: November 5, 2025)

**Complete Features:**
- ✅ Single-page website with all 9 sections fully implemented
- ✅ Hand-drawn SVG illustrations (palm trees, meditation figure, backwater landscape)
- ✅ Sage green (#8b9d87) color palette with warm cream backgrounds
- ✅ Lora and Montserrat typography with proper hierarchy
- ✅ 6 amenity cards (Bedroom, Dining, Yogashala, Chill-out, Connectivity, Animals)
- ✅ 6 activity cards (Yoga, Kayaking, Swimming, Art, Nature, Meditation)
- ✅ Pricing section with ₹6,000-10,000 per night display
- ✅ Contact form with validation and success messaging
- ✅ Fully responsive design (mobile hamburger menu, tablet/desktop layouts)
- ✅ Interactive elements (navigation hover effects, scroll-to-top button, smooth scrolling, fade-in animations)
- ✅ All inline code in single index.html file for easy deployment

**Deployment Ready:**
The website is ready for GitHub + Cloudflare Pages hosting. Simply push to GitHub and connect to Cloudflare for automatic deployment.

**Optional Future Enhancements:**
- Form submission backend (Formspree, Netlify Forms, etc.)
- Favicon and social preview metadata
- Additional high-quality photography
- Analytics integration (Google Analytics, Plausible, etc.)
- Map integration for location visualization