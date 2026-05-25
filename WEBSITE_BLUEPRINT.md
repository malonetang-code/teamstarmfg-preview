# Teamstar Manufacturing Website Blueprint

This document records the long-term website structure for Teamstar Manufacturing / 群新工业. It is intended to keep future Codex and OpenClaw edits aligned.

## Positioning

- Primary positioning: custom industrial knives and machine blades from drawings, samples, or equipment applications.
- Audience: procurement teams, engineers, equipment manufacturers, distributors, and industrial end users.
- Tone: concrete, factory-like, technical, and verifiable. Avoid vague marketing language.
- Core proof points from project materials:
  - Wei Qun group history begins in Taiwan, with 40+ years of industry background.
  - Shenzhen production base established in 1990.
  - Zhangzhou Qunxin established in 2024.
  - ISO 9001:2015 certification.
  - Product scope includes woodworking, food processing, plastic recycling, paper, textile/apparel, hand tools, stationery, and custom-shaped industrial knives.
  - Capability scope includes heat treatment, grinding, CNC machining, laser cutting, inspection lab, OEM/ODM, sample validation, and batch production.

## Information Architecture

Current single-page portal structure:

1. `#home` - Hero and positioning
   - Main value proposition
   - RFQ and product directory CTAs
   - High-level proof points

2. Gateway section
   - Product directory
   - Custom manufacturing
   - Manufacturing capabilities
   - SEO resource hub

3. `#products` - Product directory
   - Application-based categories now
   - Future detail pages later

4. `#custom` - Custom manufacturing process
   - Requirement check
   - Material and process advice
   - Prototype validation
   - Batch production and records

5. `#capabilities` - Manufacturing capabilities
   - Heat treatment and laser
   - CNC and grinding
   - Inspection lab
   - Explicit placeholders for missing specs and report samples

6. `#quality` - Quality system
   - ISO
   - In-house heat treatment
   - Inspection equipment
   - Batch consistency

7. `#company` - Company and base story
   - Timeline
   - Factory facts
   - Data points marked as pending confirmation when needed

8. `#resources` - SEO resource placeholders
   - Material guides
   - Blade type guides
   - Industry applications
   - Cases and FAQs

9. `#contact` - RFQ contact
   - Contact details
   - Formspree contact form
   - RFQ data checklist

## Future SEO Page Plan

When the site moves beyond one page, split the following into dedicated URLs:

- `/products/woodworking-knives/`
- `/products/food-processing-knives/`
- `/products/plastic-crusher-blades/`
- `/products/paper-slitting-knives/`
- `/products/textile-cutting-knives/`
- `/products/custom-industrial-blades/`
- `/capabilities/heat-treatment/`
- `/capabilities/precision-grinding/`
- `/capabilities/inspection-lab/`
- `/materials/hss-vs-tool-steel-vs-carbide/`
- `/industries/woodworking/`
- `/industries/food-processing/`
- `/industries/plastic-recycling/`
- `/rfq/custom-industrial-knife-drawing-checklist/`

## Visual System

- Style direction: Swiss industrial catalog / technical manufacturing portal.
- Color system:
  - Ink: `#101820`
  - Navy: `#102f49`
  - Deep navy: `#071520`
  - Gold accent: `#b8944f`
  - Light background: `#f4f6f8`
  - Border: `#d8dee6`
- Typography:
  - Latin: IBM Plex Sans
  - Chinese: Noto Sans SC
- Layout rules:
  - Use grid, borders, real photos, and restrained typography.
  - Avoid oversized rounded cards, decorative gradients, emoji icons, and excessive shadow.
  - Prefer concrete tables/cards with technical labels.

## Placeholder Rules

Use visible placeholders only when the information is not confirmed. Do not invent:

- Hardness ranges by material
- Heat treatment equipment specifications
- Inspection report samples
- Customer names or case results
- Delivery lead times
- Export percentages or market-share claims

Current placeholders in `index.html` are intentional and should be replaced only when real confirmed data is available.

## Multilingual and SEO Notes

- The current static page uses `data-lang="zh"` and `data-lang="en"` on one URL.
- For stronger multilingual SEO later, use separate URLs such as `/` and `/en/`, then add `hreflang` annotations and language-specific canonical URLs.
- Keep visible copy concrete and keyword-relevant, but do not keyword-stuff.
- Structured data currently covers Organization, WebSite, and ItemList. Add Product, FAQ, and Breadcrumb schema only after real detail pages exist.
