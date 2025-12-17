# Capstone Portfolio Project - AI Instructions

## Project Overview
A simple, single-page HTML5 portfolio application for showcasing capstone project materials. Built with vanilla HTML, CSS, and JavaScript—no frameworks or build tools.

## Architecture & Structure
- **Single-page application**: All functionality in `index.html`
- **No backend**: Pure client-side JavaScript for file previews and link creation
- **Embedded styling**: All CSS inline in `<style>` tag for portability
- **Self-contained**: No external dependencies or CDN links

## Key Features
1. **Video Showcase**: File upload with HTML5 `<video>` preview using `URL.createObjectURL()`
2. **PDF Documentation**: File upload with `<iframe>` preview for PDF display
3. **External Resources**: Dynamic link creation from user input with URL validation

## Code Patterns & Conventions

### File Handling
```javascript
// Pattern: Object URLs for file preview
const file = e.target.files[0];
const fileURL = URL.createObjectURL(file);
element.src = fileURL;
element.style.display = 'block';
```

### Styling Approach
- Centered content with `.container` max-width 900px
- Section-based layout with consistent padding (20-40px)
- Dashed borders for file inputs to indicate drop zones
- Responsive iframe/video sizing: `width: 100%`

### JavaScript Events
- `change` listeners on file inputs for immediate preview
- `click` handlers for button actions
- `keypress` listeners for Enter key shortcuts

## Development Workflow
1. **Local testing**: Open `index.html` directly in browser (no server needed)
2. **File paths**: Uses `file://` protocol when opened locally
3. **No build step**: Edit HTML and refresh browser

## Browser Compatibility
- Modern browsers (Chrome, Firefox, Edge, Safari)
- Requires ES6 support (arrow functions, const/let)
- Uses HTML5 File API and Object URLs

## Common Tasks
- **Add new section**: Duplicate `.section` div, update ID attributes, add event listeners
- **Style changes**: Modify inline CSS in `<style>` tag
- **Security**: Uses `rel="noopener noreferrer"` for external links
