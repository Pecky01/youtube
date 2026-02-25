# Copilot Instructions for the YouTube Clone Project

## Project Overview
This project is a static YouTube-like web page built with HTML and CSS. It is designed for UI/UX prototyping and does not include JavaScript or backend logic. The main focus is on layout, responsive design, and visual mimicry of YouTube's interface.

## Key Files and Structure
- `index.html`, `second.html`: Main HTML files for different page layouts.
- `main.css`, `second.css`: Core CSS files for styling respective HTML pages.
- No JavaScript, build tools, or frameworks are present.

## Layout and Styling Patterns
- Uses `position: fixed` for the header to keep it visible while scrolling. All main content containers (e.g., `.vid-wall`, `.video-gallery`) must include a `margin-top` or `padding-top` equal to the header's height to avoid overlap.
- Sidebars use `position: fixed` and require main content to have a `margin-left` matching the sidebar's width to prevent overlap.
- Flexbox is the primary layout mechanism (`display: flex; flex-direction: row/column;`).
- Class naming follows BEM-like conventions (e.g., `.video-description`, `.bottom-right-part`).

## Developer Workflow
- No build or test commands are required; open the HTML files directly in a browser to view changes.
- All dependencies are loaded via CDN (Google Fonts, Remix Icon).
- For new UI sections, add HTML structure and corresponding CSS. Keep layout consistent with existing patterns.

## Project-Specific Conventions
- Keep all CSS for a page in its respective CSS file (e.g., `second.html` uses `second.css`).
- Use semantic HTML where possible, but prioritize matching YouTube's visual structure.
- Avoid inline styles; use classes for all styling.
- Responsive design is not enforced but is encouraged for new contributions.

## Examples
- To add a new fixed sidebar, use `position: fixed; left: 0; top: [header height];` and update main content's `margin-left`.
- To prevent header overlap, always add `margin-top: [header height];` to the main content container.

## Reference
- See `second.html` and `second.css` for the most complete example of layout and styling patterns.

---
For questions about layout or conventions, review the existing HTML/CSS or ask for clarification.
