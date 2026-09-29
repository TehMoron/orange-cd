Orange Cyberdefense Netherlands — unofficial redesign concept

This is an independent front-end concept built from scratch using the public Orange Cyberdefense Netherlands website as a content and brand reference.

Current direction — warm light mode
- One warm canvas (#FFFAF0) is used across the page, sidebar, cards, popovers and dialogs.
- Near-black (#0B0B0B) replaces pure black for headings and dark controls.
- Orange (#FF7900) remains the primary brand accent.
- Sections are separated with spacing, borders and typography rather than alternating near-white backgrounds.
- Corner rounding is intentionally restrained.
- Motion stays subtle and reduced-motion preferences are respected.

UI system
The project remains plain HTML, CSS and JavaScript. It does not install shadcn/ui directly because shadcn/ui targets React/Tailwind projects. Instead, this concept borrows the strongest shadcn/ui design-system patterns and implements them natively:
- Semantic CSS tokens for background, foreground, primary, muted, accent, border, input, ring and sidebar states.
- One radius scale shared by buttons, cards, inputs, sheets and popovers.
- Consistent button variants and icon sizing.
- Sidebar composition with separate header, content and footer areas.
- Sheet-style expanded navigation with focus trapping, Escape handling and restored focus.
- Command-style search dialog with keyboard navigation and a / shortcut.
- Popover-style country selector with explicit open/closed state.
- Line-tab behavior for the hero carousel, including arrow-key, Home and End keyboard navigation.
- Item-group treatment for service rows rather than unnecessary floating cards.
- Badge treatment for content labels.
- Shared focus-visible rings and interaction states across controls.

Interaction details
- Hero CTA buttons use a fixed content grid on desktop so every slide keeps the CTA in the same position.
- Hero autoplay pauses while the carousel is hovered or keyboard-focused and can be paused manually.
- Search and navigation overlays close with Escape and keep keyboard focus contained while open.
- Country, search and navigation overlays close each other instead of stacking.
- Sidebar menu buttons expose aria-expanded state.
- Mobile navigation uses the same off-canvas/sidebar language and avoids horizontal overflow.

Technical
- Plain HTML, CSS and JavaScript.
- No framework, build step or package install is required.
- Open index.html directly in a browser.
- Public Orange Cyberdefense images are loaded remotely, so an internet connection is required for those visuals.
- Links for pages not yet rebuilt locally still point to the current public Orange Cyberdefense site.

Files
- index.html
- styles.css
- script.js
- README.txt

This project is unofficial and is not affiliated with or endorsed by Orange or Orange Cyberdefense.
