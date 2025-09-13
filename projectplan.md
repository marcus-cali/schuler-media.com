# Schuler Media Minimalist Redesign Plan

## Design Inspiration
Based on Thinking Machines Lab website - ultra-minimalist, no boxes, clean typography, subtle animations

## Core Design Principles
- **No boxes or cards** - Content flows naturally on the page
- **Generous whitespace** - Let content breathe
- **Subtle animations** - Gentle floating effect on main header
- **Typography-first** - Text is the primary design element
- **Monochromatic palette** - Mostly black/gray text on white
- **No visual clutter** - Remove all unnecessary design elements

## Visual Direction
- **Background**: Pure white (#ffffff)
- **Text**: Dark gray/black hierarchy
- **Accent**: Minimal use of single accent color (if any)
- **Typography**: Clean serif for headings, sans-serif for body
- **Layout**: Centered, single column, max-width content
- **Spacing**: Generous padding between sections

## Implementation Tasks

### Phase 1: Foundation & Typography
- [ ] Strip all existing boxes, cards, and backgrounds
- [ ] Implement clean typography system (serif + sans-serif pairing)
- [ ] Set up minimal color palette (black, grays, white)
- [ ] Create generous spacing system
- [ ] Remove all borders and unnecessary dividers

### Phase 2: Hero Section with Floating Animation
- [ ] Create minimal hero with "SCHULER MEDIA" as main element
- [ ] Implement subtle up/down floating animation (CSS keyframes)
- [ ] Add tagline below in smaller, lighter text
- [ ] Remove all background colors/gradients
- [ ] Center everything with ample whitespace

### Phase 3: Content Sections - No Boxes
- [ ] Rewrite publications section without cards (text-only blocks)
- [ ] Services as simple text paragraphs with headers
- [ ] Recent work as minimal list items
- [ ] Remove all hover effects on containers
- [ ] Use typography and spacing for hierarchy only

### Phase 4: Subtle Interactions
- [ ] Add gentle hover effects on links only
- [ ] Implement smooth scroll behavior
- [ ] Create minimal button styles (text with underline)
- [ ] Add subtle fade-in on scroll (optional)
- [ ] Ensure all animations are slow and subtle

### Phase 5: Polish
- [ ] Fine-tune typography scales and line heights
- [ ] Adjust spacing for perfect vertical rhythm
- [ ] Optimize for mobile (maintain simplicity)
- [ ] Remove any remaining visual noise
- [ ] Test animation performance

## Technical Specifications

### Typography
- Headings: Georgia or similar serif, large scale
- Body: System sans-serif or Inter
- Sizes: Limited to 3-4 sizes maximum
- Line height: Generous (1.6-1.8 for body)

### Animation Details
- Main header float:
  - Duration: 4-6 seconds
  - Movement: 10-20px vertical
  - Easing: ease-in-out
  - Infinite loop

### Layout
- Max content width: 680-760px
- Centered single column
- No sidebars or multi-column layouts
- Sections separated by whitespace only

### Color Palette
```css
--text-primary: #1a1a1a;
--text-secondary: #666;
--text-light: #999;
--background: #ffffff;
--accent: #0066cc; /* optional, minimal use */
```

## What to Remove
- All card designs and boxes
- Background colors on sections
- Borders and dividers
- Complex hover effects
- Shadow effects
- Gradient backgrounds
- Multiple column layouts on desktop
- Decorative elements

## Success Metrics
- Achieves "invisible design" - content is the focus
- Page feels calm and uncluttered
- Typography creates clear hierarchy
- Subtle animation adds life without distraction
- Maintains professional credibility through simplicity

## Implementation Order
1. Strip down existing design to basics
2. Implement typography system
3. Add floating header animation
4. Restructure content without boxes
5. Fine-tune spacing and details

## Review Section

### Completed Changes

**Phase 1: Foundation & Typography ✓**
- Implemented system font stack matching Thinking Machines style
- Removed all boxes, cards, and visual containers
- Set up minimal color palette (black, grays, white)
- Created generous spacing system with max-width 720px

**Phase 2: Hero with Floating Animation ✓**
- Created minimal hero with "SCHULER MEDIA" floating gently up/down
- Added 6-second animation cycle with 15px movement
- Simplified tagline and description
- Removed all background colors

**Phase 3: Content Sections Without Boxes ✓**
- Converted all sections to pure text blocks
- Removed hover effects on containers
- Used typography hierarchy only (uppercase small headers)
- Made links simple underlined text

**Phase 4: Polish ✓**
- Fine-tuned spacing and typography
- Ensured consistent minimalist aesthetic
- Maintained mobile responsiveness
- All animations are subtle and smooth

### Key Design Decisions
- Used system fonts for optimal performance
- Single column layout with 720px max-width
- Uppercase section headers in small size (14px)
- Minimal link styling with opacity hover effect
- Pure white background with dark gray text

### Result
The site now achieves an ultra-minimalist aesthetic inspired by Thinking Machines, with focus entirely on content and subtle typography. The floating "SCHULER MEDIA" header adds life without distraction.