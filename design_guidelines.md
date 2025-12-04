# Design Guidelines: Advanced Airbnb Clone

## Design Approach
**Reference-Based Design** - Drawing inspiration from Airbnb's modern, clean aesthetic with emphasis on high-quality imagery, generous whitespace, and intuitive user flows.

## Core Design Principles
- **Image-First Philosophy**: Properties showcase through large, high-quality photography
- **Clean & Spacious**: Generous padding and breathing room between elements
- **Trust-Building**: Prominent ratings, reviews, and verification indicators
- **Seamless Booking Flow**: Intuitive calendar interaction and clear pricing breakdown

## Typography System
**Fonts**: 
- Primary: 'Circular' or similar (Poppins, Inter as alternatives)
- Weights: 400 (regular), 500 (medium), 600 (semibold), 700 (bold)

**Hierarchy**:
- Hero Headlines: text-4xl to text-6xl, font-semibold
- Property Titles: text-xl, font-semibold
- Section Headers: text-2xl to text-3xl, font-semibold
- Body Text: text-base, font-normal
- Captions/Metadata: text-sm, text-gray-600
- Prices: text-lg to text-2xl, font-semibold

## Layout System
**Spacing Primitives**: Use Tailwind units of 2, 4, 6, 8, 12, 16, 20, 24
- Cards/Components: p-4 to p-6
- Section Padding: py-12 to py-20
- Element Gaps: gap-4, gap-6, gap-8

**Container Strategy**:
- Full-width hero: w-full
- Content sections: max-w-7xl mx-auto px-4 to px-8
- Property grids: grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4

## Component Library

### Navigation Header
- Fixed top navigation with subtle shadow on scroll
- Logo left-aligned, search bar center (desktop), user menu right
- Search bar: rounded-full with location/dates/guests inputs
- Mobile: Hamburger menu, simplified search button

### Property Cards
- Rounded corners (rounded-xl)
- Image carousel with dots indicator
- Heart icon (top-right overlay on image)
- No border, subtle shadow on hover
- Grid layout: 4 columns desktop, 2 tablet, 1 mobile
- Content: Location, rating (star + count), price per night, dates available

### Hero Section
**Large background image** showing featured destination or property
- Height: 60vh on desktop, 50vh tablet, 40vh mobile
- Centered search bar overlay with blurred background (backdrop-blur-md bg-white/90)
- Headline: "Find your next adventure" style messaging
- CTA button with blur background treatment

### Booking Calendar
- Large, prominent monthly view
- Dates: Circular selection indicators
- Disabled dates: Crossed out or greyed
- Selected range: Connected highlight between start/end dates
- Two-month view side-by-side on desktop
- Price variations displayed on hover

### Property Detail Page
- Full-width image gallery (masonry on desktop, carousel mobile)
- Two-column layout: Content left (2/3), booking card right (1/3, sticky)
- Sections: Description, Amenities (grid with icons), Location (map embed), Reviews
- Booking card: Date selector, guest dropdown, price breakdown, "Reserve" button

### Booking Management Dashboard
- Card-based layout for reservations
- Each card: Property thumbnail, dates, status badge, actions
- Tabs: Upcoming, Past, Cancelled
- Action buttons: View Details, Cancel Booking, Modify Dates

### Filters & Search
- Sticky filter bar below header
- Pill-style filter buttons (rounded-full)
- Price range slider
- Amenity checkboxes in dropdown overlay
- "Pools" highlighted as featured amenity filter

### Payment Interface
- Clean breakdown: Nightly rate × nights, Service fee, Taxes
- Total emphasized with larger font
- Mock credit card input with card type icons
- Security badges and trust indicators

## Images Strategy

**Hero Section**: 
- Large scenic destination image (beach, mountains, urban skyline)
- 1920×800px minimum, optimized for web
- Slightly darkened overlay for text readability

**Property Listings**:
- Primary image per card (16:9 aspect ratio)
- Multiple images in carousel (3-5 per property)
- 800×600px minimum resolution
- Mix of exterior, interior, amenity shots

**Property Detail Gallery**:
- 8-12 high-quality images
- Featured image: Large hero (1200×800px)
- Grid of thumbnails below
- Include: Living spaces, bedrooms, bathrooms, outdoor areas, pool (when applicable)

**Category Icons/Imagery**:
- Pool illustrations for pool filter
- Amenity icons throughout

## Animations & Interactions
- Subtle hover elevations on cards (translate-y-1 shadow-lg)
- Smooth calendar date selection transitions
- Image carousel: Slide transitions
- Filter dropdown: Fade in/out
- NO distracting scroll animations

## Responsive Breakpoints
- Mobile: < 768px (single column, stacked layout)
- Tablet: 768px - 1024px (2 columns)
- Desktop: 1024px - 1280px (3 columns)
- Large Desktop: > 1280px (4 columns)

## Accessibility
- High contrast for text over images
- Keyboard navigation for calendar
- Screen reader labels for all interactive elements
- Focus indicators on all clickable elements
- Minimum touch target: 44×44px mobile

This design creates a professional, trust-inspiring booking platform with Airbnb's signature clean aesthetic and image-forward approach.