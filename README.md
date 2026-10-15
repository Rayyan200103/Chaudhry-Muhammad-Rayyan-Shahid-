# Chaudhry Muhammad Rayyan Shahid

**International Relations and International Development Professional**

Professional profile and portfolio site. Live at
**[rayyan200103.github.io/Chaudhry-Muhammad-Rayyan-Shahid-](https://rayyan200103.github.io/Chaudhry-Muhammad-Rayyan-Shahid-/)**

---

## Overview

A single-page professional profile documenting institutional experience across multilateral diplomacy, international development, and strategic communications. The site consolidates a full record of roles, academic work, professional outputs, credentials, and conference representation into one continuous document intended for recruiters, selection panels, and institutional contacts.

**Current position:** Partnerships and Communications Coordinator at MANGOma, a UK-registered international development charitable organisation, coordinating a 16+ partner NGO network across 11 countries in Sub-Saharan Africa, South Asia, Latin America, and Europe. The role continues from a Development Work Placement at the same organisation.

**Prior institutional experience** spans two divisions of Pakistan's Ministry of Foreign Affairs, the United Nations Division and the Iran and Turkey Division, including contribution to Pakistan's climate policy representation at COP29 under the UNFCCC and operational support to the SCO Islamabad Summit 2024.

**Qualifications:** Master of Arts in Global Development, University of East Anglia. Bachelor of Social Sciences in International Relations, Bahria University Islamabad.

**Independent publication:** The Chronicles, an interactive world history timeline at [thechronicles.live](https://thechronicles.live/).

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
| Outputs | `#outputs` | Ten documented professional products, plus The Chronicles publication panel |
| Competencies | `#competencies` | Nine core competencies mapped to supporting evidence |
| Credentials | `#credentials` | Awards, certifications, and professional training |
| Conferences | `#conferences` | Summits, delegations, and representation record |
| Engagement | `#engagement` | Memberships and volunteer service |
| Focus | `#focus` | Target roles, functional areas, and institutional preferences |
| Contact | `#contact` | Direct contact details and professional links |

---

## The Chronicles Panel

The Outputs section carries a standalone panel for The Chronicles, the author's independent research publication. The panel holds a scope strip of eight figures, a sectioned table of linked companion studies (Before Adam, Comparative Religion), a three-up platform feature row (248 languages, Ask Rayyan, Engagement Tracker), a specification list, a provenance line, and a direct contact block. Every figure in the strip is taken from the live publication, not estimated:

| Figure | Meaning |
| --- | --- |
| 13.8 billion years | Deep time before Adam AS |
| c. 300,000 years | Of *Homo sapiens* |
| 5,785 years | From Adam AS |
| 1 + 8 categories | Thematic band, world regions |
| 25 sub-categories | Across every region |
| 730 entries | Each one sourced |
| Dual calendar | Solar and lunar, BCE/CE and AH |
| 248 languages | Fully translatable |

The entry count on the live site is computed from the data at page load rather than hard-coded, so it must be read from the rendered page and not from the static HTML source, which carries a lower fallback value. When the figure changes, update it in the scope strip and in Competency 08, which are the only two places it appears.

---

## Technical Notes

**Architecture.** The site is a single self-contained `index.html` file of approximately 1.03 MB. There is no build step, no package manager, no framework, and no runtime dependency on any third-party library. Markup, styling, and behaviour are held in one document.

**Assets.** Sixteen photographic and document images are embedded directly as base64 data URIs rather than served from a separate directory. This removes all relative-path risk on GitHub Pages and guarantees the file renders identically wherever it is opened, including offline and when saved locally by a recipient.

**Typography.** Cormorant Garamond for display typography, served from Google Fonts. Aptos for body and interface typography, with a defined fallback stack of Inter, Segoe UI, Calibri, and Arial for systems where Aptos is unavailable. If the Google Fonts request fails, the fallback stack renders the page without layout shift.

**Scripts.** Two script elements. One is the inline behaviour script handling the anchor-navigation scroll engine, scroll-triggered reveals, animated statistic counters, the competencies accordion, the image lightbox, copy-to-clipboard controls, the back-to-top control, and pointer-tracked visual effects. The second is an `application/ld+json` block carrying Schema.org structured data, which executes nothing. All motion is progressive enhancement: with scripting disabled, the full content of the page remains readable.

**Search and social metadata.** The document declares a canonical URL, Open Graph properties including `og:url`, `og:site_name`, and `og:locale`, Twitter card properties, and a `robots` directive permitting full snippet and large image preview. The Schema.org `Person` graph records job title, employer, nationality, both degrees, languages, areas of knowledge, and `sameAs` links to LinkedIn and The Chronicles, with The Chronicles additionally described as a `WebSite` under `subjectOf`.

**Responsive behaviour.** The Outputs grid resolves to one column at 620px and below, two columns from 621px to 1040px, and three columns at 1041px and above. The lead output card spans the full row width in the three-column view only, so no row is left with a single orphaned card. The Chronicles scope strip resolves to four columns on desktop and two at 900px and below, and the companion-study cards stack to one column at 900px and below. A separate orientation rule restores the four-column strip and three-column cards in phone landscape, where width is ample but height is not.

**Browser support.** Current versions of Chrome, Edge, Safari, and Firefox on desktop and mobile.

---

## Accessibility

- Semantic HTML5 sectioning with a single `h1` and a coherent heading hierarchy
- `lang="en"` declared at document level
- Skip-to-content link as the first focusable element, verified by keyboard test from a clean page load
- Colour palette selected against WCAG AAA contrast thresholds for body text
- `prefers-reduced-motion` respected: animation and scroll effects are suppressed for users who have requested reduced motion at the system level, and all content renders at full opacity
- All substantive imagery carries descriptive alternative text, including images injected into the lightbox at runtime
- Accordion controls expose `aria-expanded`; every navigation control and every companion-study link is keyboard operable
- All external links carry `rel="noopener"`
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
| Images missing alternative text | None |
| External links reachable | All (LinkedIn returns its standard 999 anti-bot code; the two font 404s are `preconnect` hints, not pages) |
| JSON-LD parses as valid JSON | Yes, `Person` |
| External links without `rel="noopener"` | None |
| Horizontal overflow at 360, 390, 414, 620, 768, 844, 900, 1024, 1040, 1041, 1180, 1280, 1440, 1920px | Zero at every width |
| Navigation scroll engine | Working |
| Competencies accordion | Working |
| Statistic counters | All resolve to their declared values |
| Image lightbox, open, alt text, Escape close | Working |
| Copy-to-clipboard controls | Working |
| Reduced-motion rendering | Working, no elements left hidden |
| First keyboard tab stop | Skip-to-content link |
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

**Numeral convention.** The partner-network figure carries a plus sign (16+) and is therefore written as a numeral everywhere it appears, including running prose. Other figures appear as numerals on scannable surfaces (statistics panel, At a Glance panel, scrolling marquee, search and social metadata) and are spelled out in running prose.

**Values appearing in more than one place.** The partner network figure (16+ partners across 11 countries) appears in the hero, the About narrative, the statistics panel, the At a Glance panel, the scrolling marquee, the first competency, the third focus track, and all three metadata descriptions. The funding intelligence database appears at two different counts by design: 500 entries in the current role, which is the live maintained figure, and 211 entries in the placement record, the About narrative, and the output card, which are the historical figures delivered during the placement. Do not reconcile these to a single number. The Chronicles entry count appears in the scope strip and in Competency 08.

Where imagery is replaced, the new asset must be encoded to base64 and substituted into the corresponding data URI to preserve the self-contained architecture.

---

## Contact

**Email** rayyanchaudhry03@outlook.com
**LinkedIn** [linkedin.com/in/rayyan-shahid-4169b5271](https://www.linkedin.com/in/rayyan-shahid-4169b5271)
**Pakistan, WhatsApp** +92 333 5667116

Islamabad, Pakistan | Available for international assignment

---

## Related Work

**The Chronicles**, an independent research publication presenting world history as a single interactive timeline read across eight world regions and a thematic band of twenty-five sub-categories, dated in both BCE/CE and AH, with every entry carrying a graded source apparatus.

- Timeline: [thechronicles.live](https://thechronicles.live/)
- Reader features: 248 languages, Ask Rayyan corpus search, Engagement Tracker, installable as an app
- Before Adam AS: [thechronicles.live/before_adam.html](https://thechronicles.live/before_adam.html)
- Comparative Religion: [thechronicles.live/comparative_religion.html](https://thechronicles.live/comparative_religion.html)

The same profile page is deployed to The Chronicles as `AboutMe.html`, where it is served at `thechronicles.live/aboutme`. The two files are maintained byte-identical; any change to one must be mirrored to the other in the same commit cycle. Both carry a canonical link pointing at the GitHub Pages URL, so that search engines consolidate ranking signals into a single address rather than splitting them across two identical pages.

---

© 2026 Chaudhry Muhammad Rayyan Shahid. All content, including biographical text, professional records, and imagery, is the property of the author. The source is public for transparency and portability. It is not offered for reuse, redistribution, or adaptation as a template.
