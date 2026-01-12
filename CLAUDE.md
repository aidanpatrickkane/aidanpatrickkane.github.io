# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a personal portfolio website hosted at aidanpkane.com. It's a static site built with HTML, CSS (including Tailwind CSS), and vanilla JavaScript. The site showcases personal projects, essays, and provides contact information.

## Architecture and Structure

### Directory Layout

- **Root directory**: Contains the main landing page (`index.html`) and various standalone HTML pages
- **`public/`**: Contains compiled CSS (`style.css`), additional pages, and assets
  - `images/`: Image assets including the personal headshot
  - `bookreviews/`, `golden-goose/`, `writings/`: Content subdirectories
  - Various pages: `projects.html`, `website-projects.html`, `mystuff.html`, `privacy.html`, `support.html`, `terms.html`
- **`src/`**: Contains the Tailwind CSS input file (`input.css`)
- **Subdirectories with standalone pages**:
  - `new-app/`: Essay/project page
  - `superchill/`: Project showcase page
  - `intro/`: Introduction page
  - `my-book/`: Book-related content
  - `lookin-up-privacy/`, `lookin-up-support/`: Legal/support pages for "Lookin Up" app

### CSS Architecture

The site uses a **hybrid CSS approach**:
1. **Tailwind CSS**: Configured in `tailwind.config.js`, compiled from `src/input.css` to `public/style.css`
2. **Inline styles**: Main `index.html` contains extensive custom CSS in a `<style>` tag for the hero section, spotlight effect, and responsive design

When designing a page, use custom CSS in a <style> tag.

### Key Features

**Spotlight Effect**: The main landing page features a Mercury-inspired interactive spotlight effect:
- Two layered background images (one darkened, one with radial gradient mask)
- JavaScript tracks mouse position and updates CSS mask properties
- Creates a "revealing light" effect that follows the cursor

**Responsive Design**: Breakpoint at 1130px switches from horizontal to vertical layout and hides the email form on mobile devices.

**Form Integration**: Uses Formspree (https://formspree.io/f/mandrpnr) for email contact form submissions.

## Deployment

The site is deployed to GitHub Pages (indicated by `CNAME` file). The domain `aidanpkane.com` points to this repository.

## Navigation Structure

The main nav links to:
- Home (root)
- Body of Work (https://madebykane.com - external site)
- Superchill (`./superchill/`)
- New Essay (`./new-app/`)

## Analytics

Google Analytics is integrated (ID: G-89SZK30KTZ) for tracking page views.
