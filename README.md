# musichall-andrejkoller-next

A minimalist portfolio website dedicated to musical projects and creative work. Built with modern web technologies and a focus on performance, internationalization, and clean design.

## Features

- **Server-Side Rendering** - Fast initial page loads with Next.js App Router
- **Multilingual Support** - English, German, and Russian via a custom translation context
- **Responsive Design** - Mobile-first layout with CSS Modules and custom breakpoints
- **Background Music Player** - Ambient audio playback with SiriWave visualizations
- **Masonry Gallery** - Dynamic image gallery with PhotoSwipe lightbox
- **Custom Cursor** - Animated cursor component for desktop devices
- **Contact Form** - Email submission with phone number validation via libphonenumber-js
- **Cookie Banner** - GDPR-compliant cookie consent management
- **Parallax Effects** - Scroll-driven parallax animations with Rellax
- **Google Fonts** - Cormorant, Gloock, and Rubik via `next/font`
- **Modular Architecture** - Separated Header, Footer, Menu, and layout components

## Tech Stack

- **Framework**: [Next.js 16](https://nextjs.org) (App Router)
- **Language**: JavaScript (JSX)
- **Library**: React 19
- **Styling**: CSS Modules

## Prerequisites

- Node.js 18.x or higher
- npm, yarn, pnpm, or bun

## Installation

1. Clone the repository

```bash
git clone https://github.com/andrejkoller/musichall-andrejkoller-next.git
cd musichall-andrejkoller-next
```

2. Install dependencies

```bash
npm install
```

3. Run the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## Project Structure

```
musichall-andrejkoller-next/
+-- public/
¦   +-- audios/                   # Background audio files
¦   +-- images/                   # Static images
¦   +-- locales/
¦       +-- de.json               # German translations
¦       +-- en.json               # English translations
¦       +-- ru.json               # Russian translations
+-- src/
¦   +-- app/
¦   ¦   +-- globals.css           # Global styles
¦   ¦   +-- layout.jsx            # Root layout
¦   ¦   +-- page.jsx              # Root redirect
¦   ¦   +-- [lang]/
¦   ¦   ¦   +-- layout.jsx        # Language layout with fonts
¦   ¦   ¦   +-- layout-client.jsx # Client-side layout wrapper
¦   ¦   ¦   +-- page.jsx          # Home page
¦   ¦   ¦   +-- about/            # About page
¦   ¦   ¦   +-- contact/          # Contact page
¦   ¦   ¦   +-- gallery/          # Gallery page
¦   ¦   ¦   +-- inspiration/      # Inspiration page
¦   ¦   ¦   +-- projects/         # Projects and sub-project pages
¦   ¦   +-- api/
¦   ¦       +-- send-email/
¦   ¦           +-- contact/
¦   ¦               +-- route.js  # Email API route
¦   +-- components/
¦   ¦   +-- background-music/     # Audio player with SiriWave
¦   ¦   +-- cookie-banner/        # GDPR cookie consent
¦   ¦   +-- cursor/               # Custom animated cursor
¦   ¦   +-- footer/               # Footer component
¦   ¦   +-- header/               # Header component
¦   ¦   +-- language-switcher/    # Language toggle
¦   ¦   +-- link-button/          # Reusable link button
¦   ¦   +-- menu/                 # Navigation menu
¦   +-- contexts/
¦   ¦   +-- translation-context.js
¦   +-- hooks/
¦   ¦   +-- use-translation.js
¦   +-- libs/
¦   ¦   +-- get-dictionary.js
¦   +-- providers/
¦       +-- translation-provider.jsx
+-- eslint.config.mjs             # ESLint configuration
+-- jsconfig.json                 # JS path aliases
+-- LICENSE
+-- next.config.mjs               # Next.js configuration
+-- package.json
```

## License

This project is licensed under the [MIT License](LICENSE).
