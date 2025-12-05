# Technical Context: Angular Modern Demo - Festival CIDA
*Version: 1.0*
*Created: 2025-12-03*
*Last Updated: 2025-12-03*

## Technology Stack
- **Frontend Framework:** Angular (Latest Stable, likely v19).
- **UI Library:** Angular Material (Material 3 design).
- **State Management:** Angular Signals (Local component state).
- **CSS Strategy:** SCSS (standard Angular) with Angular Material theming.
- **Build Tool:** Angular CLI (esbuild).

## Development Environment Setup
- **Node.js:** Latest LTS.
- **Package Manager:** npm.
- **IDE:** Cursor / VS Code.
- **Angular CLI:** v20.1.4.
- **Angular Version:** v20.3.15.
- **Angular Material:** v20.0.0 (compatible with Angular 20).
- **Development Server:** `ng serve` (default port 4200).

## Dependencies
- `@angular/core`, `@angular/common`, etc.: Core framework.
- `@angular/material`, `@angular/cdk`: UI Components.
- `@angular/animations`: Required for Material.

## Technical Constraints
- **Single Page:** No complex routing needed initially, though `Router` will be configured for best practices.
- **No Zoneless:** Standard Zone.js change detection for stability in this specific demo.
- **Performance:** Must load instantly; optimized assets (hero image).

## Build and Deployment
- **Build Process:** Standard `ng build`.
- **Deployment:** Local serve for presentation (`ng serve`).

## Testing Approach
- **Unit Testing:** Karma/Jasmine (Standard) - Basic component test to show "how it's done".
- **E2E Testing:** Cypress (Optional, likely skipped for simple presentation page).

