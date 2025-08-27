## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.

## Getting Started

### Prerequisites
- Node.js (version 18 or higher)
- pnpm (recommended package manager)

### Installation and Build

1. Install dependencies:
   ```bash
   pnpm install
   ```

2. Build the application:
   ```bash
   pnpm run build
   ```

3. Start the development server:
   ```bash
   pnpm run dev
   ```

## Recent Fixes

### Font Import Issue (Fixed)
- **Issue**: Build was failing with TypeScript error: `Cannot find module '@/app/ui/fonts'`
- **Root Cause**: Multiple components were importing fonts from `@/app/ui/fonts`, but the fonts file was missing
- **Solution**: Created `app/ui/fonts.ts` with proper Next.js font imports:
  - Added `lusitana` font (Lusitana from Google Fonts)
  - Added `inter` font (Inter from Google Fonts)
  - Configured with appropriate weights and subsets

The application now builds successfully with `pnpm run build`.
