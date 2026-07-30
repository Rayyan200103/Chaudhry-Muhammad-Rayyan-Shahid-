# Chaudhry Muhammad Rayyan Shahid

**International Relations and Development Professional**

Professional profile and portfolio site. Live at
**[rayyan200103.github.io/Chaudhry-Muhammad-Rayyan-Shahid-](https://rayyan200103.github.io/Chaudhry-Muhammad-Rayyan-Shahid-/)**

---

## Overview

A single-page professional profile documenting institutional experience across multilateral diplomacy, international development, and strategic communications. The site consolidates a full record of roles, academic work, professional outputs, credentials, and conference representation into one continuous document intended for recruiters, selection panels, and institutional contacts.

Current position: Projects Intern and NGOs Coordinator at MANGOma, coordinating a nine-country partner portfolio across Africa, Latin America, and Europe. Prior institutional experience spans two divisions of Pakistan's Ministry of Foreign Affairs, including contribution to Pakistan's climate policy representation at COP29 under the UNFCCC and operational support to the SCO Islamabad Summit 2024.

---

## Site Structure

The profile is organised into twelve anchored sections, each addressable by URL fragment:

| Section | Anchor | Content |
| --- | --- | --- |
| Hero | `#hero` | Positioning statement, institutional markers, contact routes |
| About | `#about` | Professional narrative, key metrics, employer summary panel |
| Experience | `#experience` | Role-by-role record with deliverables and institutional context |
| Education | `#education` | Postgraduate and undergraduate record, module results, academic leadership |
| Expertise | `#expertise` | Five areas of expertise, media and content production, digital tools, languages |
| Outputs | `#outputs` | Nine documented professional products with issuing institution |
| Competencies | `#competencies` | Nine core competencies mapped to supporting evidence |
| Credentials | `#credentials` | Awards, certifications, and professional training |
| Conferences | `#conferences` | Summits, delegations, and representation record |
| Engagement | `#engagement` | Memberships and volunteer service |
| Focus | `#focus` | Target roles, functional areas, and institutional preferences |
| Contact | `#contact` | Direct contact details and professional links |

---

## Technical Notes

**Architecture.** The site is a single self-contained `index.html` file. There is no build step, no package manager, no framework, and no runtime dependency on any third-party library. Markup, styling, and behaviour are held in one document.

**Assets.** Photographic and document imagery is embedded directly as base64 data URIs rather than served from a separate directory. This removes all relative-path risk on GitHub Pages and guarantees the file renders identically wherever it is opened, including offline and when saved locally by a recipient.

**Typography.** Cormorant Garamond for display typography, served from Google Fonts. Aptos for body and interface typography, with a defined fallback stack of Inter, Segoe UI, Calibri, and Arial for systems where Aptos is unavailable.

**Interaction.** A single inline script handles scroll-triggered reveals, animated counters, the anchor-navigation scroll engine, the section pill navigation, and pointer-tracked visual effects. All motion is progressive enhancement: with scripting disabled, the full content of the page remains readable.

**Browser support.** Current versions of Chrome, Edge, Safari, and Firefox on desktop and mobile.

---

## Accessibility

- Semantic HTML5 sectioning with a single `h1` and a coherent heading hierarchy
- `lang="en"` declared at document level
- Skip-to-content link as the first focusable element
- Colour palette selected against WCAG AAA contrast thresholds for body text
- `prefers-reduced-motion` respected: animation and scroll effects are suppressed for users who have requested reduced motion at the system level
- All substantive imagery carries descriptive alternative text
- Every navigation control is keyboard operable

---

## Deployment

The site is published through GitHub Pages from the `main` branch, repository root.

To publish an update:

1. Replace `index.html` at the repository root
2. Commit to `main`
3. GitHub Pages rebuilds automatically, typically within two minutes
4. Hard refresh the live URL with `Ctrl` + `Shift` + `R` to clear the browser cache before reviewing

No pipeline, no dependency installation, and no local server are required. The file can be opened directly in a browser for offline verification before commit.

---

## Editing Guidance

Because the profile is a single file, edits are made by locating the relevant section and amending it in place. Content sections are demarcated by their anchor identifiers, listed in the table above. Styling is centralised in the document head, so palette or typographic changes propagate across the whole page from one location.

Where imagery is replaced, the new asset must be encoded to base64 and substituted into the corresponding data URI to preserve the self-contained architecture.

---

## Contact

**Email** rayyanchaudhry03@gmail.com
**LinkedIn** [linkedin.com/in/rayyan-shahid-4169b5271](https://www.linkedin.com/in/rayyan-shahid-4169b5271)
**United Kingdom** +44 7466 710348
**Pakistan** +92 333 5667116

Norwich, England, United Kingdom | Islamabad, Pakistan

---

## Related Work

**The Chronicles**, an independent research and visualisation project presenting world history through a dual-calendar architecture with comparative religion, international relations, and philosophy integrated across the timeline.
[rayyan200103.github.io/THE-CHRONICLE](https://rayyan200103.github.io/THE-CHRONICLE/)

---

© 2026 Chaudhry Muhammad Rayyan Shahid. All content, including biographical text, professional records, and imagery, is the property of the author. The source is public for transparency and portability. It is not offered for reuse, redistribution, or adaptation as a template.
