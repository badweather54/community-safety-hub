# Copilot Instructions for AI Agents

## Project Overview
This is a static web project for the Community Safety Hub, focused on providing resources, products, education, and legal support for community safety. The main entry point is `index.html`, which contains all markup, styles, and scripts. There is no build system, backend, or package management currently present.

## Architecture & Structure
- **Single-page HTML app**: All content, styles, and scripts are embedded in `index.html`.
- **No frameworks**: No React, Vue, Angular, or server-side code. All logic is vanilla HTML/CSS/JS.
- **No external dependencies**: Only a favicon is loaded from an external URL. No npm, pip, or other package managers.
- **No API calls or dynamic data**: All data is static and hardcoded in the HTML.

## Developer Workflows
- **Debugging**: Use the VS Code launch configurations in `.vscode/launch.json` to open the site in Microsoft Edge, either by serving at `http://localhost:8080` or directly opening `index.html`.
- **Local preview**: For live preview, use a simple static server (e.g., `npx serve .` or open `index.html` directly in a browser).
- **No build/test commands**: There are no build steps, tests, or CI/CD integrations. All changes are made directly to `index.html`.

## Project-Specific Patterns
- **Styling**: All CSS is inline within a `<style>` block in `index.html`. Responsive design is handled via media queries.
- **Navigation**: Smooth scrolling and mobile navigation are implemented with vanilla JS in a `<script>` block.
- **Product/Education Cards**: Use `.product-grid`, `.product-card`, `.educational-grid`, and `.resource-card` classes for layout and styling.
- **Analytics/Affiliate Tracking**: Example code for Google Analytics event tracking is present but commented out. No real analytics integration yet.

## Integration Points
- **Edge Debugging**: `.vscode/launch.json` provides three launch configurations for Edge, including direct file opening and localhost preview.
- **Favicon**: Uses an emoji favicon from an external CDN.

## Conventions
- **All code in one file**: Make all changes in `index.html` unless adding new static assets.
- **No external JS/CSS**: Do not introduce frameworks or libraries unless explicitly requested.
- **Accessibility**: Navigation and layout are designed to be mobile-friendly and accessible.

## Examples
- To add a new product card, edit the `.product-grid` section in `index.html`.
- To update navigation, modify the `<nav>` block and related JS in `index.html`.
- To change launch/debug settings, update `.vscode/launch.json`.

---
For questions about missing workflows or unclear conventions, ask the user for clarification before making major changes.
