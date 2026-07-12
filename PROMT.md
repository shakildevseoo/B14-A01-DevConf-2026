# Prompt: DevConf 2026 — Hackathon Timeline Section

## Context
I'm building a landing page for **DevConf 2026**, a developer conference with the tagline "Code. Connect. Create." The page already has:
- A dark navy hero section with a photo background and a blue "Register Now" CTA button
- A light "Meet the Speakers" section with a card grid
- A "Secure Your Spot" pricing section with 3 tiers (Standard, Pro — dark navy highlighted, Team)
- A placeholder box reading "Something Missing? Generate a relevant section with AI" that needs to be replaced

**Existing color system:**
- Primary accent: royal blue, used on buttons and links
- Dark navy background, used in the hero and the "Pro" pricing card
- Light backgrounds elsewhere on the page
- Bold, heavy sans-serif headings; muted gray body text on dark backgrounds

## Task
Design and build a **Hackathon Details** section to replace the placeholder, using the site's existing dark navy + blue palette so it feels native to the page rather than bolted on.

The section should include:
1. A short eyebrow label + heading + one-line subtitle introducing the hackathon
2. A horizontal connected timeline of the event day, with:
   - A circular icon marker for each step (outlined, blue border, dark fill)
   - A thin horizontal connector line running behind all the markers
   - A short label under each marker: **Kickoff (Fri 6PM) → Build → Submissions (Sun 10AM) → Demos → Awards**
3. Icons from Font Awesome solid style (already loaded via CDN — no new icon library)
4. Fully responsive: on mobile, the timeline should stack vertically with the connector line running down the left side instead of across
5. Visible focus states for accessibility, and respect `prefers-reduced-motion`

## Style requirements
- Reuse the site's existing navy tones and blue accent — do not introduce new colors
- Circular markers should look like outlined badges: dark navy fill, blue border, blue icon
- Keep spacing and typography consistent with the rest of the page (same heading weight/size scale)
- Sizing (marker size, gaps, font sizes) should be left to sensible design judgment rather than fixed to exact values, since it needs to match my own existing CSS system
- Deliver clean, external HTML + CSS only (no inline styles, no framework), scoped under a single parent class (e.g. `.hackathon`) using BEM-style naming so it doesn't collide with existing CSS

## Deliverable
One HTML block for the timeline section, and a separate external CSS file, ready to paste into the existing page in place of the placeholder.