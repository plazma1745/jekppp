# Overview

This is a Jekyll-powered static business website theme called "Serif" designed for professional service companies. The site appears to be localized for a Russian metal cutting business in Zlatoust, offering plasma and laser cutting services. It's built as a modern, responsive business website with content management capabilities through Jekyll collections and layouts.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Static Site Generation
The project uses Jekyll 4.2+ as its static site generator, providing a fast, secure, and SEO-optimized website. Jekyll compiles Markdown content and Liquid templates into static HTML files that can be served from any web server or CDN.

## Content Management Structure
The site employs Jekyll's collection system for organized content management:
- **Services Collection** (`_services/`): Individual service pages with markdown content and front matter metadata
- **Team Collection** (`_team/`): Team member profiles with images, job titles, and biographical information
- **Data Files** (`_data/`): Structured JSON data for features, social links, and navigation menus

## Template System
The architecture uses a hierarchical layout system:
- **Base Layout** (`default.html`): Master template with HTML structure, meta tags, and common elements
- **Specialized Layouts**: Page-specific templates for home, services, contact, and team pages
- **Component Includes**: Reusable template fragments for header, footer, navigation, and content blocks

## Frontend Architecture
The site uses a modern responsive design approach:
- **Bootstrap 4.6**: Grid system and utility classes for responsive layout (minimal import strategy)
- **SCSS Preprocessing**: Modular stylesheet architecture with variables and mixins
- **Mobile-First Design**: Responsive breakpoints with hamburger navigation for mobile devices
- **Performance Optimization**: Minimal JavaScript footprint with only essential interactive elements

## Content Localization
The site content is localized for Russian-speaking users with Cyrillic text throughout the navigation, content, and service descriptions. The theme maintains its English template structure while supporting Russian content.

## SEO and Analytics Integration
Built-in SEO optimization includes:
- Meta tag management through Jekyll front matter
- Open Graph and Twitter Card support
- Google Analytics integration with environment-based configuration
- Structured data support through Jekyll's metadata system

## Deployment Architecture
The site is designed for multiple deployment targets:
- **Netlify**: Primary hosting platform with built-in CI/CD
- **GitHub Pages**: Alternative hosting option with Jekyll native support
- **Static Hosting**: Can be deployed to any static file hosting service

The build process compiles all templates, processes SCSS, and generates a complete static site in the `_site` directory.

# External Dependencies

## Core Dependencies
- **Jekyll 4.2+**: Static site generator and templating engine
- **Ruby**: Runtime environment for Jekyll
- **Bundler**: Ruby dependency management

## Frontend Libraries
- **Bootstrap 4.6**: CSS framework (grid system and utilities only)
- **Google Fonts**: Playfair Display font family via CDN
- **SCSS/Sass**: CSS preprocessing for modular stylesheets

## Analytics and Tracking
- **Google Analytics**: Website traffic tracking and analysis
- **Google Tag Manager**: Tag management system integration

## Content Management
- **Netlify CMS (Decap CMS)**: Headless CMS for content editing (configured via `admin/` directory)
- **Markdown**: Content authoring format with front matter metadata
- **Liquid**: Jekyll's templating language for dynamic content

## Hosting and Deployment
- **Netlify**: Primary hosting platform with automatic deployment
- **GitHub Pages**: Alternative hosting option
- **Git**: Version control system for content and code management

## Development Tools
- **VS Code Extensions**: Prettier and Stylelint for code formatting and linting
- **Node.js**: Development toolchain for frontend asset processing