# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal portfolio website for Emanuel Giannattasio - Data Engineer & ETL Developer. Static landing page designed for GitHub Pages hosting.

## Technology Stack

- **HTML5** - Semantic markup structure
- **CSS3** - Custom properties, Flexbox, Grid, responsive design
- **Vanilla JavaScript** - Interactions, typing effect, scroll animations
- **Google Fonts** - Inter (UI), JetBrains Mono (code)

## Repository Structure

```
/
├── index.html      # Main landing page
├── styles.css      # All styles (variables, components, responsive)
├── script.js       # JavaScript interactions
├── cv/             # CV documents (PDF, DOCX)
└── CLAUDE.md       # This file
```

## Development

No build system required. Open `index.html` directly in browser or use any local server:

```bash
# Python
python -m http.server 8000

# Node.js (if npx available)
npx serve
```

## GitHub Pages Deployment

1. Push to GitHub repository
2. Go to Settings > Pages
3. Select branch `main` and root folder `/`
4. Site will be available at `https://<username>.github.io/<repo-name>/`

## Key Sections

- **Hero** - Introduction with typing effect animation
- **About** - Professional summary, DRY/KISS principles
- **Experience** - Timeline of work history (Prisma, ACL-Group, Strata, etc.)
- **Skills** - Technical skills grid (Python, AWS, Airflow, SQL, etc.)
- **Projects** - Links to Streamlit apps and GitHub
- **Education** - Academic background and certifications
- **Contact** - Email, LinkedIn, GitHub links

## Design System

CSS custom properties in `:root` define colors, spacing, typography. Dark theme with blue accent (#3b82f6). Mobile-first responsive breakpoints at 1024px, 768px, 480px.
