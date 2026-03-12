# Repository Guidelines

## Project Structure & Module Organization
This repository is a lightweight static site for GitHub Pages.

- `index.html`: Main page content and section structure.
- `styles.css`: All visual styling and responsive behavior.
- `README.md`: Editing and deployment instructions.
- `Logos/`: Brand assets (use SVG/PNG variants as needed).
- `Proposed UVAS Officer Structure.docx`: Source of record for officer language.
- `uvas_elections_github_pages_instructions.md`: Original implementation brief.

Keep content changes in `index.html` and presentation changes in `styles.css`.

## Build, Test, and Development Commands
No build step is required.

- `python3 -m http.server 8000`
  - Serve the site locally at `http://localhost:8000`.
- `rg -n "YOUR_NOMINATION_FORM_LINK|YOUR_VOTING_FORM_LINK" index.html`
  - Verify placeholder links were replaced.
- `rg -n "<section|id=\"" index.html`
  - Quick structure check for anchor targets/navigation.

## Coding Style & Naming Conventions
- Use 2-space indentation in HTML/CSS.
- Prefer semantic HTML (`section`, `nav`, `main`, `footer`, lists).
- Keep CSS class names descriptive and lowercase with hyphens (e.g., `action-callout`, `role-entry`).
- Preserve plain JavaScript-free behavior unless a clear need appears.
- Keep editable copy directly in HTML; do not hide key content in scripts.

## Testing Guidelines
Automated tests are not configured for this repository.

Before submitting changes:
- Validate layout on desktop and mobile widths.
- Verify all nav links scroll to the correct section IDs.
- Confirm external form links and logo paths resolve.
- Confirm officer wording matches the source document when editing role text.

## Commit & Pull Request Guidelines
No commit history is present in this folder yet. Use this convention going forward:
- Commit format: `type: short imperative summary`
  - Examples: `feat: reorder timeline above positions`, `fix: correct appointed roles copy`
- Keep commits focused (content vs. styling vs. deployment docs).

PRs should include:
- What changed and why.
- Screenshots for desktop + mobile when UI/layout is affected.
- Any content-source note (for example, “copied verbatim from officer docx”).
