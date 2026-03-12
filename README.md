# UVAS Elections Website (Vercel)

This repository contains a modern, conversion-focused static website for UVAS elections, optimized for free hosting on Vercel.

## Project Files

- `index.html` - Page content, UI structure, and Vercel Analytics script.
- `styles.css` - Visual design, typography, grid layouts, and responsive queries.
- `archive/` - Folder containing previous design iterations (V1 and V2) for historical reference.
- `20250917_Meet the Firms_KE_*.jpg` - Official event photography used throughout the layout.

## 1) Editable Action Links

Open `index.html` to update the call-to-action buttons in the bottom section. 
Currently:
- **Nomination Form:** Links to the active Microsoft Form.
- **Voting Form:** Styled with a `.btn-disabled` class and an inactive href (`javascript:void(0)`) since voting is not open yet. Once voting opens, update the URL and delete the `btn-disabled` class to make it green and clickable.

## 2) Edit Content Sections

In `index.html`, content is organized logically into semantic sections:

- **Hero (`#top`):** The primary call to action, timeline status card, and background image integration. Update the academic year (e.g. 2026-2027) inside the subtitle `<p>`.
- **About (`#about`):** The value proposition and benefits list, paired with an inline event photo.
- **Roles (`#roles`):** Each position is a `<div class="role-card">...</div>` block. You can safely edit the `<h3>` titles and `<ul>` duties without breaking the grid structure.

## 3) Analytics Integration

The website implements official Vercel Analytics for tracking visits. Because this is a static HTML site without a build framework, it uses a script tag injected directly into the `<head>` of `index.html`:
`<script defer src="/_vercel/insights/script.js"></script>`

You **do not** need to install any `npm` packages. Vercel automatically powers this script when the site is deployed.

## 4) Publish on Vercel

1. Log into your account at [Vercel.com](https://vercel.com).
2. Click **Add New Project**.
3. Import this GitHub repository (`uvas_elections_site`).
4. Leave all settings default (Framework preset: `Other`, Build Command: `None`).
5. Click **Deploy**.

Moving forward, simply running `git push` from your terminal will trigger Vercel to automatically rebuild and update your live URL within seconds!

## Notes

- The site is fully static (no backend/database required).
- The hero section uses `20250917_Meet the Firms_KE_0164.jpg` as the background natively mapped inside `styles.css`.
- If your forms require Microsoft authentication, keep the on-page login note in the HTML.
