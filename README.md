# Chaudhry Muhammad Rayyan Shahid

**International Relations and International Development Professional**

Professional profile and portfolio site. Live at
**[rayyan200103.github.io/Chaudhry-Muhammad-Rayyan-Shahid-](https://rayyan200103.github.io/Chaudhry-Muhammad-Rayyan-Shahid-/)**

---

## Overview

A single-page professional profile documenting institutional experience across multilateral diplomacy, international development, and strategic communications. The site consolidates a full record of roles, academic work, professional outputs, credentials, and conference representation into one continuous document intended for recruiters, selection panels, and institutional contacts.

**Current position:** Partnerships and Communications Coordinator at MANGOma, a UK-registered international development charity, coordinating a sixteen-partner NGO network across eleven countries in Sub-Saharan Africa, South Asia, Latin America, and Europe. The role continues from a Development Work Placement at the same organisation.

**Prior institutional experience** spans two divisions of Pakistan's Ministry of Foreign Affairs, including contribution to Pakistan's climate policy representation at COP29 under the UNFCCC and operational support to the SCO Islamabad Summit 2024.

**Qualifications:** Master of Arts in Global Development, University of East Anglia. Bachelor of Social Sciences in International Relations, Bahria University Islamabad.

---

## Site Structure

Twelve anchored sections, each addressable by URL fragment:

| Section | Anchor | Content |
| --- | --- | --- |
| Hero | `#hero` | Positioning statement, institutional markers, contact routes |
| About | `#about` | Professional narrative, eight key metrics, At a Glance panel |
| Experience | `#experience` | Five roles with deliverables and institutional context |
| Education | `#education` | Degrees in full title, module results with distinctions, placement report, academic leadership |
| Expertise | `#expertise` | Five areas of expertise, media production, digital tools, languages |
| Outputs | `#outputs` | Ten documented professional products, plus The Chronicles |
| Competencies | `#competencies` | Nine core competencies mapped to supporting evidence |
| Credentials | `#credentials` | Awards, certifications, and professional training |
| Conferences | `#conferences` | Summits, delegations, and representation record |
| Engagement | `#engagement` | Memberships and volunteer service |
| Focus | `#focus` | Target roles, functional areas, and institutional preferences |
| Contact | `#contact` | Direct contact details and professional links |

---

## Technical Notes

**Architecture.** The site is a single self-contained `index.html` file of approximately 1.02 MB. There is no build step, no package manager, no framework, and no runtime dependency on any third-party library. Markup, styling, and behaviour are held in one document.

**Assets.** Sixteen photographic and document images are embedded directly as base64 data URIs rather than served from a separate directory. This removes all relative-path risk on GitHub Pages and guarantees the file renders identically wherever it is opened, including offline and when saved locally by a recipient.

**Typography.** Cormorant Garamond for display typography, served from Google Fonts. Aptos for body and interface typography, with a defined fallback stack of Inter, Segoe UI, Calibri, and Arial for systems where Aptos is unavailable. If the Google Fonts request fails, the fallback stack renders the page without layout shift.

**Interaction.** A single inline script handles the anchor-navigation scroll engine, scroll-triggered reveals, animated statistic counters, the competencies accordion, the image lightbox, copy-to-clipboard controls, the back-to-top control, and pointer-tracked visual effects. All motion is progressive enhancement: with scripting disabled, the full content of the page remains readable.

**Responsive behaviour.** The Outputs grid resolves to one column at 620px and below, two columns from 621px to 1040px, and three columns at 1041px and above. The lead output card spans the full row width in the three-column view only, so no row is ever left with a single orphaned card at any width.

**Browser support.** Current versions of Chrome, Edge, Safari, and Firefox on desktop and mobile.

---

## Accessibility

- Semantic HTML5 sectioning with a single `h1` and a coherent heading hierarchy
- `lang="en"` declared at document level
- Skip-to-content link as the first focusable element, verified by keyboard test
- Colour palette selected against WCAG AAA contrast thresholds for body text
- `prefers-reduced-motion` respected: animation and scroll effects are suppressed for users who have requested reduced motion at the system level, and all content renders at full opacity
- All substantive imagery carries descriptive alternative text, including images injected into the lightbox at runtime
- Accordion controls expose `aria-expanded`; every navigation control is keyboard operable
- Lightbox closes on the Escape key

---

## Verification

The deployed file was checked in a headless Chromium browser before release. Results:

| Check | Result |
| --- | --- |
| JavaScript runtime errors | None |
| Console errors | None (excluding the sandboxed font request, which resolves normally when hosted) |
| Duplicate element IDs | None |
| Broken in-page anchors | None |
| Broken images | None |
| Horizontal overflow at 360, 390, 414, 620, 768, 844, 900, 1024, 1040, 1041, 1180, 1280, 1440, 1920px | Zero at every width |
| Navigation scroll engine | Working |
| Competencies accordion | Working |
| Statistic counters | All resolve to their declared values |
| Image lightbox, open, alt text, Escape close | Working |
| Copy-to-clipboard controls | Working |
| Reduced-motion rendering | Working |
| HTML tag balance across all element types | Balanced |

---

## Deployment

The site is published through GitHub Pages from the `main` branch, repository root.

To publish an update:

1. Replace `index.html` at the repository root. The filename must be lowercase; GitHub Pages runs on a case-sensitive filesystem and will not serve `Index.html` as the directory default.
2. Commit to `main`
3. GitHub Pages rebuilds automatically, typically within two minutes
4. Hard refresh the live URL with `Ctrl` + `Shift` + `R` to clear the browser cache before reviewing

No pipeline, no dependency installation, and no local server are required. The file can be opened directly in a browser for offline verification before commit.

---

## Editing Guidance

Because the profile is a single file, edits are made by locating the relevant section and amending it in place. Content sections are demarcated by their anchor identifiers, listed in the table above. Styling is centralised in the document head, so palette or typographic changes propagate across the whole page from one location.

Two values appear in more than one place and must be changed together to keep the page internally consistent: the **partner network figure** (sixteen partners across eleven countries) appears in the hero, the About narrative, the statistics panel, the At a Glance panel, the scrolling marquee, the first competency, and the third focus track; the **funding intelligence database count** appears in the current role, the placement record, the About narrative, and its own output card.

Where imagery is replaced, the new asset must be encoded to base64 and substituted into the corresponding data URI to preserve the self-contained architecture.

---

## Contact

**Email** rayyanchaudhry03@gmail.com
**LinkedIn** [linkedin.com/in/rayyan-shahid-4169b5271](https://www.linkedin.com/in/rayyan-shahid-4169b5271)
**Pakistan** +92 333 5667116
**United Kingdom** +44 7466 710348

Islamabad, Pakistan | Available for international assignment

---

## Related Work

**The Chronicles**, an independent research and visualisation project presenting world history through a dual-calendar architecture with comparative religion, international relations, and philosophy integrated across the timeline.
[rayyan200103.github.io/THE-CHRONICLE](https://rayyan200103.github.io/THE-CHRONICLE/)

The same profile page is also deployed there as `AboutMe.html`. The two files are maintained byte-identical; any change to one must be mirrored to the other in the same commit cycle.

---

© 2026 Chaudhry Muhammad Rayyan Shahid. All content, including biographical text, professional records, and imagery, is the property of the author. The source is public for transparency and portability. It is not offered for reuse, redistribution, or adaptation as a template.
