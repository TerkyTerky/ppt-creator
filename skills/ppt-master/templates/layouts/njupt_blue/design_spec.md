---
template_id: njupt_blue
category: general
summary: Clean corporate blue theme with card-based layouts, hub-and-spoke diagrams, and data-analysis pages. Suitable for business reports, product presentations, and executive briefings.
keywords: [blue, corporate, clean, data-driven, card-layout, hub-spoke]
primary_color: "#042C91"
canvas_format: ppt169
replication_mode: fidelity
placeholders:
  01_cover: ["{{TITLE}}", "{{SUBTITLE}}", "{{AUTHOR}}", "{{DESCRIPTION}}"]
  02_toc: ["{{TOC_ITEM_1_TITLE}}", "{{TOC_ITEM_1_DESC}}", "{{TOC_ITEM_2_TITLE}}", "{{TOC_ITEM_2_DESC}}", "{{TOC_ITEM_3_TITLE}}", "{{TOC_ITEM_3_DESC}}", "{{TOC_ITEM_4_TITLE}}", "{{TOC_ITEM_4_DESC}}"]
  03_chapter: ["{{CHAPTER_NUM}}", "{{CHAPTER_TITLE}}", "{{CHAPTER_DESC_1}}", "{{CHAPTER_DESC_2}}", "{{CHAPTER_DESC_3}}"]
  04_content: ["{{PAGE_TITLE}}", "{{CARD_1_TITLE}}", "{{CARD_2_TITLE}}", "{{CARD_3_TITLE}}", "{{CARD_1_LINE_1}}", "{{CARD_1_LINE_2}}", "{{CARD_1_LINE_3}}", "{{CARD_1_LINE_4}}", "{{CARD_1_LINE_5}}", "{{CARD_1_LINE_6}}", "{{CARD_2_LINE_1}}", "{{CARD_2_LINE_2}}", "{{CARD_2_LINE_3}}", "{{CARD_2_LINE_4}}", "{{CARD_2_LINE_5}}", "{{CARD_2_LINE_6}}", "{{CARD_3_LINE_1}}", "{{CARD_3_LINE_2}}", "{{CARD_3_LINE_3}}", "{{CARD_3_LINE_4}}", "{{CARD_3_LINE_5}}", "{{CARD_3_LINE_6}}", "{{PAGE_NUM}}"]
  05_content_bullet: ["{{PAGE_TITLE}}", "{{HUB_TITLE_LINE_1}}", "{{HUB_TITLE_LINE_2}}", "{{NODE_1_TITLE}}", "{{NODE_1_DESC}}", "{{NODE_2_TITLE}}", "{{NODE_2_DESC}}", "{{NODE_3_TITLE}}", "{{NODE_3_DESC}}", "{{NODE_4_TITLE}}", "{{NODE_4_DESC}}", "{{PAGE_NUM}}"]
  06_content_data: ["{{PAGE_TITLE}}", "{{CHART_TITLE}}", "{{CHART_PLACEHOLDER}}", "{{ANALYSIS_1_LABEL}}", "{{ANALYSIS_1_LINE_1}}", "{{ANALYSIS_1_LINE_2}}", "{{ANALYSIS_1_LINE_3}}", "{{ANALYSIS_2_LABEL}}", "{{ANALYSIS_2_LINE_1}}", "{{ANALYSIS_2_LINE_2}}", "{{ANALYSIS_2_LINE_3}}", "{{PAGE_NUM}}"]
  07_ending: ["{{THANK_YOU}}", "{{ENDING_SUBTITLE}}", "{{CONTACT_INFO}}"]
---

# Blue Universal — Design Specification

## I. Template Overview

A clean, corporate blue theme derived from a 19-slide business deck. Mixed theme mode: chapter and ending pages use a full-bleed deep-blue gradient (`#042C91` → `#1E36A4`), while content pages sit on a light `#F8FAFC` background. At a glance, the template is recognized by its numbered circle badges, blue-bordered white cards with soft drop shadows, floating low-opacity ellipse accents, and triangular geometric decorations on dark pages.

## II. Color Scheme

| Role | HEX | Usage |
|------|-----|-------|
| Primary | `#042C91` | Chapter/cover/ending backgrounds, card borders, hub center fill |
| Accent | `#06398B` | Numbered circles, label pills, decorative triangles, shadow tints |
| Light accent | `#B9D3FC` | Decorative gradient bars, secondary text on dark backgrounds |
| Background | `#F8FAFC` | Content page background |
| Text dark | `#262626` | Body text on light pages |
| Text gray | `#A5A5A5` | Chart placeholder label, page numbers |
| White | `#FFFFFF` | Text on dark backgrounds, card fills |

Gradient on dark pages: `#042C91` (top) → `#1E36A4` at 0.5 opacity (bottom).

## III. Typography

The template uses a mixed Chinese font stack intentionally diverging from the default:

| Role | Stack |
|------|-------|
| Cover/chapter titles | `Source Han Sans SC, sans-serif` |
| Chapter number | `Microsoft YaHei, Source Han Sans SC, sans-serif` |
| Chapter bullets | `Source Han Serif CN Heavy, Source Han Sans SC, sans-serif` |
| Content body | `Microsoft YaHei Light, Source Han Sans SC, sans-serif` |

All title-level and UI-label text uses `font-weight="bold"`.

## IV. Signature Design Elements

**Dark-page decorative system** (cover, chapter, ending): floating white ellipses at 10% opacity placed at asymmetric positions; horizontal colored bars using a `#B9D3FC` → transparent gradient; small triangular arrow accents (`#06398B`) in groups of three at page corners.

**Card drop-shadow**: content cards use a custom SVG filter (`feGaussianBlur` stdDeviation 4–8, `feOffset` dy 2–4, flood color `#06398B` at 8–12% opacity). Applied via `filter="url(#cardShadow)"` on card background rects.

**Numbered badges**: circles (r=42–44px) filled with `#042C91`, centered above card titles or used as TOC item markers. White bold number inside.

**Logo**: placed at top-right (x=985, y=19) on cover, chapter, and ending pages. Source: `logo.png` bundled with the template.

## V. Page Roster

| File | Type | Description |
|------|------|-------------|
| `01_cover.svg` | Cover | Full-bleed blue gradient, decorative concentric circles and floating ellipses. Title + subtitle + author + description text block at left. Logo at top-right. |
| `02_toc.svg` | TOC | Four numbered items (01–04) in a vertical list layout. Each has a circle badge, title, and description line. Blue gradient background with right-side decorative circle/arc. |
| `03_chapter.svg` | Chapter | Full-bleed blue gradient with large right-side decorative circle and rotated gradient arc. Chapter number centered mid-page, large title below, three bullet descriptors in a horizontal row. |
| `04_content.svg` | Content (3-card grid) | Light background. Page title + underline at top. Three equal-width cards in a horizontal row, each with a numbered circle badge, card title, divider line, and 6 lines of body text. Blue-bordered white cards with drop shadows. |
| `05_content_bullet.svg` | Content (hub-and-spoke) | Light background. Central circular hub with two-line title. Four satellite nodes (top/right/bottom/left) with numbered circles (01–04), node titles, and descriptions. Concentric ring around hub center. |
| `06_content_data.svg` | Content (chart + analysis) | Light background. Left half: white card with chart title and placeholder area (dashed border). Right half: two stacked analysis cards with blue pill labels and 3-line text blocks each. |
| `07_ending.svg` | Ending | Full-bleed blue gradient overlay. Decorative horizontal bars and triangular accents. Large "Thank You" and subtitle text, contact info line below. Logo at top-right. |

## VI. Assets

| File | Dimensions | Usage |
|------|-----------|-------|
| `logo.png` | 267×67 | Top-right logo on cover, chapter, and ending pages |
