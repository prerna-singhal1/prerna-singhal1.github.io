# README for main.html

## Overview
This project is a single-file personal portfolio website built with HTML, CSS, and a small amount of vanilla JavaScript.

The page is designed as a modern, high-contrast profile site for **Prerna Singhal**, including:
- Hero intro
- About section
- Projects showcase
- Experience timeline
- Awards and achievements
- Community impact
- Fellowships and programs
- Contact links

## File Covered
- `main.html` - Complete page markup, styling, and scroll animation script.

## How to Run
1. Open `main.html` directly in any modern browser, or
2. Use VS Code Live Server for auto-refresh while editing.

No build tools or dependencies are required.

## Page Structure
The page is organized in this order:
1. Fixed navigation bar
2. Hero section (`#hero`)
3. About (`#about`)
4. Projects (`#projects`)
5. Experience (`#experience`)
6. Awards (`#awards`)
7. Impact (`#impact`)
8. Programs (`#programs`)
9. Contact (`#contact`)
10. Footer

## Styling Notes
- CSS is embedded in the `<style>` block inside `main.html`.
- Theme colors and font variables are defined in `:root`.
- Layout uses:
  - CSS Grid for cards/section arrangements
  - Flexbox for nav, CTA groups, and contact rows
- A responsive breakpoint at `max-width: 900px` adjusts layout for mobile.

## JavaScript Behavior
A small script at the bottom of the file uses `IntersectionObserver` to apply staggered fade-in + upward motion when elements enter the viewport.

Observed elements include:
- Project cards
- Award cards
- Program cards
- Timeline items
- Impact number cards
- Skill tags

## Common Edits
### Update Content
- Edit text directly inside each section in `main.html`.

### Update Links
- Social links are in the Hero CTA and Contact section.

### Update Theme
- Change values under `:root` to alter the color palette and typography globally.

### Add New Project
- Duplicate one `.project-card` block inside the `#projects .projects-grid` container.

## Browser Compatibility
Works in modern browsers that support:
- CSS Grid
- Flexbox
- `IntersectionObserver`

For very old browsers, animations may not run as expected.

## Maintenance Tips
- Keep section IDs consistent with nav anchor links.
- Reuse existing utility classes (`.btn`, `.ptag`, `.skill-tag`, etc.) to maintain visual consistency.
- If the page grows much larger, consider splitting CSS/JS into separate files for easier maintenance.
