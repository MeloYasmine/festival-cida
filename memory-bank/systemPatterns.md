# System Patterns: Festival CIDA Landing Page
*Version: 1.0*
*Created: 2025-12-03*
*Last Updated: 2025-12-03*

## Architecture Overview
Single-page application with a clean, component-based architecture following Angular modern best practices. The application is structured to showcase Standalone Components, Signals, and Material Design theming.

## Key Components
- **AppComponent (Root):** Main application shell, handles routing (if needed) and global layout structure.
- **HeroComponent / HomeComponent:** Full-screen landing page component containing the visual hero section with background, title, and event information.
- **Theme Configuration:** Angular Material custom theme matching the Festival CIDA visual identity (purple, yellow, white palette).

## Design Patterns in Use
- **Standalone Components:** All components use `standalone: true` (no NgModules).
- **Signal-based Reactivity:** Component state managed with Angular Signals for reactive updates.
- **Material Design 3:** Using Angular Material with custom theming to match the Festival CIDA brand colors.
- **Component Composition:** Simple parent-child relationship (App -> Hero/Home) demonstrating clean separation of concerns.

## Data Flow
Minimal data flow for a static landing page:
- Component initialization → Render static content with Material theming
- Future: If animations or interactions are added, Signals will handle state changes reactively

## Key Technical Decisions
- **Standalone Architecture:** Eliminates NgModule boilerplate, aligns with Angular's future direction.
- **Material Theming:** Custom theme allows brand consistency while leveraging Material's component library.
- **Single Component Structure:** Simple component hierarchy keeps the demo focused and easy to understand during presentation.

## Component Relationships
```
AppComponent (root)
  └── HeroComponent / HomeComponent
      ├── Background (CSS/SCSS with gradient/texture)
      ├── Title Section ("1º Festival CIDA - Ciência, Design & Ancestralidade!")
      └── Event Details (if needed: date, time, location)
```

## Visual Design System (Inspired by Festival CIDA Poster)
- **Primary Color:** Rich Purple (background, main canvas)
- **Accent Color:** Bright Yellow (highlights, title emphasis)
- **Text Color:** White (primary text)
- **Style:** Modern, vibrant, graphic design with potential for subtle textures/gradients
- **Typography:** Clean, sans-serif (Material typography system)

