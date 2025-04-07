# Vizee Web – Internal Developer Documentation

## 1. Project Overview
**Project**: Vizee Web  
**Type**: Internal Website Project for Vizee Creative Studio  
**Goal**: Showcase Vizee's digital design and branding services with a modern, fast, and responsive site.

---

## 2. Tech Stack & Tooling
- Vite (build tool for fast development and optimized builds)
- HTML/CSS with Framer-generated structure
- Prettier (code formatter)
- Git (version control)
- Node.js for dependency management
- Fonts via Google Fonts and Framer assets

---

## 3. NPM Scripts
These scripts are defined in `package.json`:

```json
"scripts": {
  "dev": "vite",
  "build": "vite build",
  "preview": "vite preview",
  "format": "prettier --write ."
}
```

- `dev`: Starts the local development server  
- `build`: Produces a production-ready build  
- `preview`: Serves the build locally for testing  
- `format`: Applies Prettier formatting across the codebase

---

## 4. File Structure & Notes
- `index.html`: Root HTML, contains meta tags, Framer-generated scripts, and layout structure.
- Project is likely hosted on Framer based on metadata.
- Static site, can be extended with JavaScript for interactivity or deployed as-is.

---

## 5. Local Setup Guide

```bash
# 1. Clone the repository
git clone <REPO_URL> && cd vizee-web

# 2. Install dependencies
npm install

# 3. Start development server
npm run dev
```

---

## 6. Code Formatting & Standards
- Use `npm run format` before commits.
- Follow Prettier configuration to maintain consistent code style.
- Avoid manual changes to `index.html` if managed by Framer.

---

## 7. Deployment
- Site is buildable using `vite build`.
- Built files are output in `dist/` folder and can be hosted via Vercel, Netlify, GitHub Pages, or Framer.
- Canonical and OpenGraph metadata in `index.html` point to: [https://expansive-lot-537569.framer.app](https://expansive-lot-537569.framer.app)

---

## 8. Potential Improvements
- Modularize styles or move to SCSS/PostCSS for scalability.
- Introduce deployment script for automated Vercel/Netlify pushes.