# Brand Style Guide - RootCause.sh

## Colour Palette

### Light Theme

#### Primary Colours
- **Primary Background**: `#FFFFFF` (Pure white)
- **Secondary Background**: `#F6F7F9` (Very light grey)
- **Primary Colour**: `#FFD700` (Bright gold)
- **Accent Colour**: `#FFE55C` (Bright light gold)
- **Secondary Colour**: `#E6C200` (Brighter darker gold)
- **Primary Text**: `#151517` (Soft black)
- **Secondary Text**: `#53535A` (Medium grey)
- **Borders**: `#E5E7EB` (Light grey)

### Dark Theme

#### Primary Colours
- **Primary Background**: `#0B0B0C` (Deep black)
- **Secondary Background**: `#121214` (Very dark grey)
- **Primary Colour**: `#FFE55C` (More intense bright gold)
- **Accent Colour**: `#FFF176` (More intense bright light gold)
- **Secondary Colour**: `#FFD54F` (Brighter darker gold)
- **Primary Text**: `#F2F2F3` (Soft white)
- **Secondary Text**: `#B4B4B6` (Light grey)
- **Borders**: `#1E1E20` (Dark grey)

## Typography

### Fonts
- **Primary Font**: Inter (Google Fonts)
  - Available weights: 400, 500, 600, 700, 800, 900
- **Monospace Font**: JetBrains Mono (Google Fonts)
  - Available weights: 400, 500, 600, 700

### Text Sizes
- **Hero Text**: `clamp(3rem, 8vw, 6rem)` (Responsive)
- **Line height**: 1.5 (general), 1.1 (hero)

## Visual Effects

### Gradients
- **Gradient Text**: `linear-gradient(135deg, var(--color-primary), var(--color-accent))`
- **Direction**: 135 degrees (diagonal)

### Animations
- **Fade In Up**: 0.6s ease-out
- **Slow Pulse**: 3s cubic-bezier(0.4, 0, 0.6, 1) infinite

### Blur Effects
- **Soft Backdrop Blur**: 8px
- **Extra Soft Backdrop Blur**: 2px

## Interactive States

### Hover
- **Accent Hover**: Changes to accent colour
- **Border Hover**: Changes to border colour
- **Text Hover**: Changes to primary text colour
- **Primary Hover**: Changes to primary colour

### Focus
- **Focus Ring**: `rgb(var(--color-primary) / 0.5)` with 2px offset
- **Focus Border**: Primary colour

### Selection
- **Selection Background**: `rgb(var(--color-primary) / 0.2)`
- **Selection Colour**: Primary text colour

## Custom Scrollbar

### Light Theme
- **Width**: 6px
- **Track**: Surface colour (`#F6F7F9`)
- **Thumb**: Border colour (`#E5E7EB`)
- **Thumb Hover**: Secondary text colour (`#53535A`)

### Dark Theme
- **Track**: Surface colour (`#121214`)
- **Thumb**: Border colour (`#1E1E20`)
- **Thumb Hover**: Secondary text colour (`#B4B4B6`)

## CSS Implementation

Colours are implemented using custom CSS variables:

```css
:root {
  --color-bg: #FFFFFF;
  --color-surface: #F6F7F9;
  --color-primary: #FFD700;
  --color-accent: #FFE55C;
  --color-secondary: #E6C200;
  --color-text: #151517;
  --color-text-secondary: #53535A;
  --color-border: #E5E7EB;
}

.dark {
  --color-bg: #0B0B0C;
  --color-surface: #121214;
  --color-primary: #FFE55C;
  --color-accent: #FFF176;
  --color-secondary: #FFD54F;
  --color-text: #F2F2F3;
  --color-text-secondary: #B4B4B6;
  --color-border: #1E1E20;
}
```

## Logo and Visual Elements

### Adaptive Logo
- **Light Theme**: `light-icon-512.png`
- **Dark Theme**: `dark-icon-512.png`
- **Transition**: Smooth between themes (0.3s)
- **No effects**: No shadows or rounded borders

### Buttons
- **Primary Button**: Yellow background with black text for maximum contrast
- **Alternative Button**: Yellow text with yellow border, hover with yellow background and black text
- **Contrast**: Optimised for accessibility (black text on yellow)

## Usage Notes

- The brand uses a bright gold colour scheme as the primary colour
- Contrast is optimised for accessibility in both themes
- Colours adapt automatically between light and dark themes
- Visual consistency is maintained across all interactive states
- Buttons use black text on yellow background for optimal legibility
