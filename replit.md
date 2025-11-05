# Sarvodaya Retreats Website

## Overview

Sarvodaya Retreats is a single-page static website for a backwater retreat sanctuary near Varkala, Kerala. The project is designed as a self-contained artistic showcase featuring hand-drawn SVG illustrations, organic layouts, and a peaceful aesthetic. The entire website is contained in a single HTML file for maximum simplicity and ease of deployment.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture

**Single-File Architecture**: The entire website is contained within `index.html`, including all CSS (embedded in `<style>` tags) and JavaScript (embedded in `<script>` tags). This monolithic approach was chosen for:
- Maximum simplicity and portability
- Zero build process or bundling requirements
- Easy deployment to any static hosting service
- Elimination of file path/dependency issues

**Design System**: Uses CSS custom properties (`:root` variables) for consistent theming:
- Color palette: Sage green (#8b9d87), warm cream (#f5f1ed), taupe, charcoal
- Typography: Google Fonts (Lora for headings/body, Montserrat for UI elements)
- No CSS frameworks - all styling is custom and hand-crafted

**Component Structure**: Semantic HTML5 sections:
- Hero banner with call-to-action
- About section (philosophy)
- Space section (amenities showcase)
- Experiences section (activities)
- Pricing information
- Location details
- Contact form
- Footer

**Responsive Design**: Mobile-first approach using CSS media queries, ensuring seamless experience across devices without JavaScript-based responsive handling.

### Form Handling

**Contact Form Integration**: Uses Formspree (third-party form backend service) to handle form submissions:
- No backend server required
- Form posts directly to Formspree endpoint via HTTP POST
- Client-side validation with vanilla JavaScript
- Success/error handling built into the page
- Sends emails to sarvodayaretreats@gmail.com

**Rationale**: Formspree was chosen over building a custom backend because:
- The website is purely static with no server-side requirements
- Formspree's free tier (50 submissions/month) is sufficient for a small retreat business
- Eliminates need for server infrastructure, databases, or email service configuration
- Provides spam protection and email delivery without complexity

### Deployment Strategy

**Static Hosting**: Designed for GitHub Pages + Cloudflare Pages deployment:
- No build step required
- No output directory processing
- Direct serving of HTML file
- Free hosting with CDN benefits

**Alternative**: The single-file architecture makes it deployable to any static host (Netlify, Vercel, simple S3 bucket, etc.) without modification.

### JavaScript Architecture

**Vanilla JavaScript**: No frameworks (React, Vue, etc.) used because:
- Interactivity requirements are minimal (form validation, scroll effects)
- Reduces page weight and improves load times
- Eliminates build tooling complexity
- All functionality can be achieved with simple DOM manipulation

**Features Implemented**:
- Smooth scroll navigation
- Form validation and submission handling
- Fade-in animations on scroll (Intersection Observer API)
- Interactive hover effects

## External Dependencies

### Third-Party Services

**Formspree** (https://formspree.io)
- Purpose: Contact form backend and email delivery
- Integration: HTTP POST to form endpoint
- Configuration: Endpoint URL must be added to form action attribute
- Email destination: sarvodayaretreats@gmail.com
- Free tier: 50 submissions/month

### External Assets

**Google Fonts API**
- Fonts loaded: Lora (serif, weights 400/500/600, regular/italic) and Montserrat (sans-serif, weights 300/400/500)
- Preconnected to fonts.googleapis.com and fonts.gstatic.com for performance
- Display strategy: swap (ensures text remains visible during font load)

### Hosting Services

**GitHub** (https://github.com)
- Purpose: Source code hosting and version control
- Repository visibility: Must be public for free Cloudflare Pages hosting

**Cloudflare Pages** (implied deployment target)
- Purpose: Static site hosting with CDN
- Build settings: No build command, root directory `/`
- Alternative: Any static hosting service (Netlify, Vercel, GitHub Pages)

### Development Dependencies

**None** - The project intentionally has zero build dependencies, bundlers, or package managers. No Node.js, npm, webpack, or similar tools are required.