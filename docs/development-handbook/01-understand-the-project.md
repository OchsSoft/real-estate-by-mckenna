# Understand the project

## The product and its current limits

This repository contains a public real-estate portfolio and contact page. Visitors can learn about McKenna, view selected property-marketing examples, read the site's positioning, and follow contact, scheduling, or social links. It is a static website: its authored HTML, styles, images, and browser script are delivered directly to the visitor. There is no application server that processes leads and no administrative dashboard hidden behind the page.

The entire interactive implementation is in `index.html`. Assets under `assets/` provide portrait, listing, and supporting imagery. A small slideshow rotates through eight authored slide entries. Its data is editorial content in JavaScript, not a live listing feed. A sold or under-contract headline reflects the checked-in text; it does not query a real-estate service or verify current availability.

This is an independent business website. It does not require the AIOS stack to start or remain useful. If operational visibility is added later, keep the website's public content and client-facing identity independent from private internal tools.

## What visitors can expect

The page has navigation anchors for top, about, work, and contact. The work section presents a sold-home slideshow with previous, next, and dot controls. Contact actions hand off to email, an external scheduling service, or a social site. The website does not itself record that an inquiry was sent or an appointment was booked.

| Capability | State at this baseline |
| --- | --- |
| Portfolio and brand content | Authored HTML and images. |
| Carousel | Browser JavaScript with timed and manual navigation. |
| Lead form/database | Absent. |
| Live MLS or listing synchronization | Absent. |
| Scheduling | External link; destination owns completion. |
| User accounts or payments | Absent. |
| Build system/package installation | Absent. |

A static site is not inherently unfinished. It is a good fit for a small brochure or portfolio when contact is intentionally external. Its limitations need to be clear so future development adds only the capabilities the business actually needs.

## Reading with implementation confidence

This handbook explains the committed implementation and safe continuation work. It does not attest that every external destination is currently available or that the live domain serves this exact revision. Verify those separately during a release review. The source reference pins this edition so you can tell which facts came from code and which are proposed improvements.
