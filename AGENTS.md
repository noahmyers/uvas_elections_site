# Repository Guidelines

## Project Structure & Module Organization
This repository is a lightweight static site designed to be hosted on Vercel (free tier).

- `index.html`: Main page content, section structure, and Vercel Analytics tracking script.
- `styles.css`: All visual styling, grid layouts, and responsive behavior.
- `README.md`: Editing and deployment instructions.
- `Logos/`: Brand SVG assets.
- `archive/`: Previous layout iterations (V1 and V2) preserved for reference.
- `20250917_Meet the Firms_KE_0164.jpg` and `...0403.jpg`: Professional event photography used for the hero background and feature sections.
- `Proposed UVAS Officer Structure.docx`: Source of record for officer language.

Keep content changes in `index.html` and presentation changes in `styles.css`. No build framework (like Next.js or React) is used.

## Analytics & Hosting
- **Hosting:** Hosted via Vercel. Pushing to the `main` branch automatically triggers a deployment. No build command is necessary since it is a plain HTML site.
- **Analytics:** Vercel Analytics is implemented via a pure HTML `<script defer src="/_vercel/insights/script.js"></script>` tag in the `<head>` of `index.html`. Do *not* run `npm install` packages.

## Build, Test, and Development Commands
No build step is required.

- `python3 -m http.server 8000`
  - Serve the site locally at `http://localhost:8000`.
- `rg -n "<section|id=\"" index.html`
  - Quick structure check for anchor targets/navigation.

## Coding Style & Naming Conventions
- Use 2-space indentation in HTML/CSS.
- Prefer semantic HTML (`section`, `nav`, `main`, `footer`, lists).
- Keep CSS class names descriptive and lowercase with hyphens (e.g., `role-card`, `btn-primary`, `btn-disabled`).
- Preserve plain JavaScript-free behavior unless a clear need appears.
- Keep editable copy directly in HTML; do not hide key content in scripts.

## Testing Guidelines
Automated tests are not configured for this repository.

Before submitting changes:
- Validate layout on desktop and mobile widths.
- Verify all nav links scroll to the correct section IDs.
- Check that the hero gradient overlay (`linear-gradient`) provides sufficient contrast over the background photography.
- Confirm officer wording matches the source document when editing role text.

## Commit & Pull Request Guidelines
- Commit format: `type: short imperative summary`
  - Examples: `feat: add vercel analytics script`, `design: update hero background image`
- Keep commits focused (content vs. styling vs. deployment docs).

PRs should include:
- What changed and why.
- Screenshots for desktop + mobile when UI/layout is affected.
- Any content-source note (for example, “copied verbatim from officer docx”).
