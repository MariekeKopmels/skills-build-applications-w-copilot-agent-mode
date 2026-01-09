Title: Update layout for improved usability and responsiveness

Summary

The current project layout (frontend and docs) needs updates to improve visual hierarchy, responsive behavior, and consistency across pages. This issue requests a small redesign and specific layout fixes to make the app easier to use on desktop and mobile.

Background / Problems

- Several pages look cramped on small screens and don't follow a consistent spacing/grid system.
- Navigation and primary CTAs (buttons/links) are not prominent enough.
- Some images and content blocks don't scale cleanly at narrow widths.
- The README/docs layout could better showcase the app screenshot and feature list.

Proposed changes

1. Adopt a simple responsive grid (e.g., 12-column) or consistent container widths with clear breakpoints (mobile, tablet, desktop).
2. Increase spacing (margins/padding) around main content and headings for better scannability.
3. Make primary CTAs visually distinct (color/size) and ensure they remain accessible on mobile.
4. Ensure images (like `docs/octofitapp-small.png`) are responsive (max-width: 100%; height: auto) and accompanied by appropriate captions.
5. Standardize header/nav layout across pages and ensure the mobile nav collapses into a clear hamburger menu if needed.
6. Update `README.md` or `docs/` pages to surface the app screenshot and feature bullets near the top.

Acceptance criteria

- Layout looks balanced on desktop (>= 1024px) and mobile (<= 480px).
- Navigation and primary CTA are visible and usable without horizontal scrolling on small screens.
- Images scale correctly and don't overflow their containers.
- README/docs updated to highlight screenshot and short feature summary.

Files to check / update

- Frontend layout files (wherever header, nav, and main content are implemented)
- `README.md` and files under `docs/` (e.g., `docs/octofit_story.md`)
- Any CSS or tailwind/SCSS files used for spacing and breakpoints

Notes / Suggestions

- If the project uses a CSS framework (Bootstrap, Tailwind, etc.), prefer using the framework's responsive utilities and container classes.
- Start with a single page (e.g., landing or main dashboard) as a pattern, then apply sitewide.
- Add a small screenshot or before/after example in the PR for visual review.

Priority: medium

If you'd like, I can open a PR that implements the above changes for the main landing/page and add a before/after screenshot. Let me know which page you want updated first.