# Stratalock USA - Foundation Repair Website

A modern, responsive website for Stratalock, a foundation repair company specializing in deep soil injection technology.

## Project Structure

```
stratalock-usa/
├── public/
│   └── images/
│       ├── stratalock-logo.svg (placeholder - replace with actual logo)
│       └── hero-workers.jpg (add your hero image: 621x775px)
├── src/
│   ├── components/
│   │   ├── Button.astro
│   │   ├── Header.astro
│   │   └── Hero.astro
│   ├── layouts/
│   │   └── BaseLayout.astro
│   └── pages/
│       └── index.astro
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

## Getting Started

### 1. Install Dependencies

```bash
npm install
```

### 2. Add Your Images

Place the following images in the `public/images/` directory:

- **Logo**: `stratalock-logo.svg` (approximately 185px wide)
- **Hero Image**: `strata-lock-hero-v1.webp` (recommended size: 621x775px)
- **About Section Image**: `about-worker.svg` (518x428px) - replace SVG placeholder with actual .jpg/.webp
- **Team Avatars**: `team-avatar.svg` (40x40px each) - replace with actual team member photos
- **Service Images**:
  - `service-residential.svg` (410x280px)
  - `service-commercial.svg` (410x280px)
  - `service-infrastructure.svg` (410x280px)
  - Replace SVG placeholders with actual photos
- **Why Choose Us Image**: `why-choose-us.svg` (518x633px) - replace SVG placeholder with actual photo
- **CTA Gallery Images**: (194x194px each)
  - `cta-gallery-1.svg`
  - `cta-gallery-2.svg`
  - `cta-gallery-3.svg`
  - `cta-gallery-4.svg`
  - Replace SVG placeholders with actual project photos
- **Case Study Images**:
  - `case-study-1.svg` (577x385px - Corona Millworks)
  - `case-study-2.svg` (240x385px vertical - Apartment Complex)
  - `case-study-3.svg` (240x385px vertical - Layne Construction)
  - `case-study-4.svg` (577x385px - Residential)
  - Replace SVG placeholders with actual project photos
- **Testimonial Image**: `testimonial-1.svg` (272x443px) - replace SVG placeholder with actual photo

### 3. Run Development Server

```bash
npm run dev
```

The site will be available at `http://localhost:4321`

### 4. Build for Production

```bash
npm run build
```

The production build will be in the `dist/` directory.

## Design Specifications

### Colors

- **Orange Primary**: #F14B00
- **Orange Accent**: #FF3B00
- **Orange Light**: #FA7523
- **Orange Dark**: #932E00
- **Background Dark 1**: #0B0B0B
- **Background Dark 2**: #161616
- **White**: #FFFFFF
- **Gray Light**: #A2A2A2
- **Gray Medium**: #7C7C7C

### Typography

- **Poppins**: Navigation, body text, buttons
- **Manrope**: Headlines, taglines
- **Inter**: Statistics

### Features

- Fully responsive (desktop, tablet, mobile)
- Sticky header with active navigation state
- Gradient CTA buttons with hover effects
- Decorative glows and grid overlays
- Image fade effects using CSS gradients
- Flexbox and Grid layout (no absolute positioning)

## Components

### Header

Sticky header with logo, navigation menu, and CTA button.

### Hero

Full-viewport hero section with:
- Two-column layout (content left, image right)
- Company statistics and features
- Main headline with gradient text effect
- CTA button and phone number
- Hero image with decorative grid overlay

### Button

Reusable button component with:
- Two sizes (small, large)
- Orange gradient background
- Hover animations

### About Section

Comprehensive about section featuring:
- Statistics bar with 4 key metrics (95% less disruption, 5+ states, 98% success rate, 15+ year warranty)
- Two-column layout with image and text content
- Team avatars with overlapping effect
- Combined experience display
- Highlighted text in headline ("solve", "stabilizing")
- Decorative orange glow in bottom-right corner

### Services Section

Showcases three main service categories:
- Alternating card layouts (content-image, image-content pattern)
- Icon boxes with service-specific icons (residential, commercial, infrastructure)
- Image with gradient overlays and decorative corner brackets
- Orange glow effects on alternating sides
- Reusable ServiceCard component for easy content management
- Fully responsive with mobile stacking

### Why Choose Us Section

Highlights company differentiators:
- Section header with tagline, headline, and stats (40+ years, 98% success rate)
- Two-column layout with dark feature box and image
- Three key features with icon boxes (Deep Soil Injection, Minimal Disruption, Engineering Expertise)
- Gradient fade on right edge of feature box
- Orange glow behind image
- Highlighted text in headline
- Data-driven feature content for easy updates

### CTA/Affordability Section

Emphasizes cost-effectiveness and drives conversions:
- Image gallery with 4 square images in alternating vertical positions
- Two-column content layout with headline and stats
- Highlighted affordability message ("30-50% Less Than Traditional Piers")
- "Get Free Estimate" CTA button with phone number
- Decorative diamond grid overlay (rotated from hero)
- Orange glow in bottom-right corner
- Purple glow with mix-blend-mode for visual interest
- Responsive gallery that adapts to mobile (2x2 grid or single column)

### Case Studies Section

Showcases real project examples with results:
- 2x2 grid of case study cards with different layout types
- Card Type 1: Full-width background image with text overlay
- Card Type 2: Split layout with vertical image and stats display
- Card Type 3: Split layout with vertical image and progress bar
- Card Type 4: Full-width background image with text overlay
- Corner bracket decorations on all images
- Orange glow effects on vertical images
- Responsive grid that adapts to single column on mobile
- Reusable CaseStudyCard component with flexible layout options
- Data-driven content for easy updates

### Testimonials Section

Displays customer testimonials and reviews:
- Three testimonial cards in a row with varying widths
- Card 1 (637px): Featured testimonial with worker image on right
- Cards 2 & 3 (323px & 313px): Text-only testimonials
- Each card features:
  - Large quotation mark icon
  - Service type title
  - Customer testimonial text
  - Customer name and location
- All cards have consistent 443px height
- Reusable TestimonialCard component supports both image and text-only layouts
- Data-driven testimonial content for easy management
- Responsive: stacks cards vertically on mobile

### Get Started Section

Final conversion-focused section before footer:
- Centered layout with all content aligned center
- "GET STARTED" tagline
- Large headline with highlighted "We Can Help." text
- Description about free assessment
- "Get Free Estimate" CTA button (reuses Button component)
- Phone number with clickable tel: link for mobile
- Three trust badges with orange checkmark icons:
  - Licensed & Insured Contractors
  - 40+ Years Combined Experience
  - Minimal Disruption Guaranteed
- Checkmarks rendered as SVG with orange stroke (#FA7523)
- Responsive: badges stack vertically or wrap on mobile
- Acts as final push for conversions

### Footer

Comprehensive footer with navigation and social links:
- Gradient background: linear-gradient(108.67deg, #111111 0%, #161616 100%)
- Three-column layout: Logo/CTA | Navigation | Social
- Stratalock logo (185px x 152px)
- Footer CTA with orange square icon and "Contact Us" button
- Navigation links (About, Services, Service Areas, Process, Case Studies)
- Social media links with arrow icons (Twitter, Instagram, LinkedIn)
- 1272px divider line separating top from bottom
- Bottom bar with:
  - Copyright: "© 2025 Stratalock."
  - Rights: "All Rights Reserved."
  - "Free Estimate" link that scrolls to top
- Hover effects on all links (gray to white transition)
- Arrow icons animate on hover (translate up-right)
- Responsive: stacks columns vertically on mobile

## Customization

### Update Navigation

Edit the `navItems` array in [src/components/Header.astro](src/components/Header.astro):

```javascript
const navItems = [
  { name: 'Home', href: '/', active: true },
  { name: 'About', href: '/about' },
  // Add more items...
];
```

### Update Colors

Modify CSS custom properties in [src/layouts/BaseLayout.astro](src/layouts/BaseLayout.astro):

```css
:root {
  --color-orange-primary: #F14B00;
  /* Update other colors... */
}
```

### Update Content

Edit the hero content in [src/components/Hero.astro](src/components/Hero.astro).

## Browser Support

- Modern browsers (Chrome, Firefox, Safari, Edge)
- CSS Grid and Flexbox support required
- CSS custom properties support required

## License

All rights reserved - Stratalock USA
