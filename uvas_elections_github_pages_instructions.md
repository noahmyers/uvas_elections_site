# Build Instructions for a GitHub Pages Election Website

## Objective
Create a clean, professional, mobile-friendly static website for the student accounting society election process. The site will be hosted on GitHub Pages and will link out to Microsoft Forms in our Microsoft 365 environment for candidate sign-up and voting.

This is meant to replace the need for a complicated SharePoint site. The webpage is only the public-facing information page. The actual forms and response collection will remain inside Microsoft 365.

## Technical Requirements
Build this as a simple static website that can be hosted directly on GitHub Pages.

Use:
- `index.html`
- `styles.css`
- `script.js` only if needed

Do **not** use a framework unless there is a strong reason. Plain HTML/CSS/JavaScript is preferred so the page is easy to edit later.

## Design Requirements
The page should look polished, university-appropriate, and modern without being flashy.

Design goals:
- clean and professional
- accounting/business student audience
- responsive on desktop and mobile
- accessible color contrast
- clear visual hierarchy
- simple navigation
- card-based layout for positions and process steps
- visually prominent call-to-action buttons

Suggested aesthetic:
- white background
- dark blue or navy accents
- subtle gray borders/shadows
- modern sans-serif font stack
- generous spacing

## Page Content and Structure
Build a single-page site with the following sections.

### 1. Header / Hero Section
Include:
- title: `UVAS Student Accounting Society Elections`
- short subtitle explaining that students can review officer roles, submit candidacy interest, and vote during the election window
- two main buttons:
  - `Run for Office`
  - `Vote in the Election`

These buttons should link to placeholder URLs that I can replace later.

Use these placeholders:
- `YOUR_NOMINATION_FORM_LINK`
- `YOUR_VOTING_FORM_LINK`

### 2. About the Election Process
Add a short section explaining:
- students can review officer positions below
- interested students may submit candidacy information through the nomination form
- after the nomination period closes, students can vote during the election window
- election results will be announced at the end-of-semester event

### 3. Officer Positions Section
Create a visually clean card layout for officer positions.

Use placeholder position cards for now:
- President
- Vice President
- Secretary
- Treasurer
- Director of Events
- Director of Membership

Each card should include:
- position title
- short placeholder description text
- optional bullet list of responsibilities

Make the content easy for me to edit later. Use obvious placeholder text where needed.

### 4. Election Timeline Section
Create a clean timeline or step-by-step section using these phases:
- `Step 1: Review positions`
- `Step 2: Submit interest to run`
- `Step 3: Student voting`
- `Step 4: Winners announced`

Use placeholder dates that I can update later. Make the dates clearly editable.

Suggested placeholder dates:
- Interest deadline: `March 27`
- Voting deadline: `April 4`
- Announcement: `April 14`

### 5. How to Participate Section
Create a simple three-step section:
1. Read the officer descriptions
2. Submit your candidacy information if you want to run
3. Vote during the election period

### 6. Call-to-Action Section
Repeat the main action buttons near the bottom of the page:
- `Submit Candidacy`
- `Vote Now`

Link them again to:
- `YOUR_NOMINATION_FORM_LINK`
- `YOUR_VOTING_FORM_LINK`

### 7. Footer
Include a simple footer with placeholder text such as:
- `Questions? Contact the faculty advisors.`
- optional placeholder email text

## Content Editing Requirements
Make the page easy for a non-web-developer to edit.

Specifically:
- keep all editable text clearly labeled in the HTML
- include comments in the HTML for places where I should replace content
- use obvious placeholder links for Microsoft Forms
- do not bury important content in JavaScript

## Deployment Requirements
Set this up so I can host it on GitHub Pages with minimal effort.

Please also create a short `README.md` that explains:
1. how to replace the Microsoft Forms links
2. how to edit officer descriptions
3. how to update dates
4. how to publish on GitHub Pages

## GitHub Pages Publishing Notes
The site should work by pushing the files to a GitHub repository and enabling GitHub Pages.

Assume deployment from the root of the repository.

## Nice-to-Have Features
Include these only if they are quick and keep the page simple:
- smooth scrolling navigation links
- subtle hover effects on cards and buttons
- a sticky top navigation bar
- a small note near the forms buttons that Microsoft login may be required to complete the forms

## Constraints
Do not build a backend.
Do not store responses on the website.
Do not require any database.
Do not use anything that would break simple GitHub Pages hosting.

## Deliverables
Please generate:
- `index.html`
- `styles.css`
- `README.md`
- `script.js` only if needed

## Acceptance Criteria
The result should:
- look professional enough for a university student organization
- be easy to host on GitHub Pages
- be easy for me to edit later
- clearly direct students to Microsoft Forms for nominations and voting
- work well on desktop and mobile

## Final Note
Keep this lightweight, clean, and practical. The goal is a good-looking webpage that I can publish quickly, not a complicated web app.

