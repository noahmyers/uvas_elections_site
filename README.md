# UVAS Elections Website (GitHub Pages)

This repository contains a simple static website for UVAS elections, designed to host directly on GitHub Pages.

## Files

- `index.html` - page content and editable text
- `styles.css` - visual design and responsive layout

## 1) Replace Microsoft Forms Links

Open `index.html` and replace all instances of:

- `YOUR_NOMINATION_FORM_LINK`
- `YOUR_VOTING_FORM_LINK`

They appear in the hero buttons and the bottom call-to-action buttons.

## 2) Edit Officer Descriptions

In `index.html`, go to the `Officer Positions` section (`id="positions"`).

Each position is a `<article class="card">...</article>` block.
You can edit:

- the title in `<h3>`
- the responsibilities in the `<ul><li>...</li></ul>` list

## 3) Update Election Dates

In `index.html`, go to the `Election Timeline` section (`id="timeline"`).
Update the text in each `<p class="date">...</p>`.

Current placeholders:

- Interest deadline: March 27
- Voting deadline: April 4
- Announcement: April 14

## 4) Publish on GitHub Pages

1. Push this repository to GitHub.
2. In GitHub, go to `Settings` -> `Pages`.
3. Under `Build and deployment`, choose:
   - `Source`: `Deploy from a branch`
   - `Branch`: `main` (or your default branch), folder `/ (root)`
4. Save.
5. GitHub will provide your live site URL.

## Notes

- The site is fully static (no backend/database required).
- The logo is loaded from `Logos/Side Stack/AccountingSociety-SideStack-Green.svg`.
- If your forms require authentication, keep the on-page login note.
