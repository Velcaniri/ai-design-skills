# Product Page UX Audit

A practical AI skill for reviewing e-commerce product pages, identifying
UX/UI problems, and turning design feedback into clear, prioritized
improvements.

## Overview

**Product Page UX Audit** helps an AI assistant evaluate product detail
pages as complete shopping experiences---not just attractive
screenshots.

It provides a structured checklist of 15 common product-page mistakes,
three optional UX enhancements, and a repeatable audit workflow. Each
finding should explain what is wrong, why it matters to shoppers, and
how to improve it.

## What it checks

The skill covers 15 common issues:

1.  Navigation icons that lose contrast over product images
2.  Poorly chosen or inconsistent product imagery
3.  Inconsistent alignment
4.  Overly bright or saturated colors
5.  Inconsistent typography
6.  Cramped labels and overloaded badges
7.  Weak product-title hierarchy
8.  Difficult-to-read description text
9.  Ratings and reviews detached from the product title
10. Inconsistent feature icons
11. Heavy divider lines
12. Unbalanced section spacing
13. Redundant price labels
14. Confusing quantity and price presentation
15. Poorly designed purchase actions

It also considers three possible enhancements:

-   Scrollable product-details cards
-   Sticky bottom purchase areas
-   Predefined quantity options

These enhancements are suggestions, not mandatory design patterns. The
skill encourages evaluating whether each one actually benefits the
product and its users.

## How it works

When given a product page, screenshot, mockup, or prototype, the
assistant should:

1.  Understand the product, audience, platform, and shopping context
    where available.
2.  Inspect the page's hierarchy, imagery, information, controls, and
    purchase flow.
3.  Identify issues that are actually present.
4.  Explain each issue and its impact on the user.
5.  Recommend a concrete correction.
6.  Prioritize the findings by severity.
7.  Separate necessary fixes from optional enhancements.
8.  Identify anything that needs further testing or cannot be verified
    from the supplied material.

The skill explicitly discourages inventing problems just to reach a
certain number of findings.

## Example prompts

Try prompts like:

-   "Audit this product page and identify its biggest UX problems."
-   "Review this e-commerce screenshot. Be specific about alignment,
    hierarchy, spacing, and typography."
-   "Find usability problems in this product detail page and prioritize
    the fixes."
-   "Critique this redesign and explain which changes would genuinely
    improve the shopping experience."
-   "Create a practical redesign plan for this product page."

## Installation

Download or clone this repository, then place `skill.md` in the skills
directory or import it using the skill-loading method supported by your
AI tool.

The exact installation path depends on the agent or platform you use.

## Repository structure

``` text
product-page-ux-audit/
├── README.md
└── skill.md
```

## Design philosophy

Good product-page design is not simply about making a screen look
cleaner. It is about helping shoppers:

-   Understand what the product is
-   Evaluate its quality and suitability
-   Find important information quickly
-   Trust what the page communicates
-   Choose options and quantities confidently
-   Understand the cost before purchasing
-   Complete the purchase without unnecessary friction

Recommendations should be specific, practical, and grounded in the
supplied design. Visual preference alone should not be presented as an
objective usability problem.

## Scope and limitations

This skill is a design-review aid, not a substitute for user research or
usability testing. A screenshot may reveal visual issues, but it cannot
confirm every interaction, accessibility behavior, responsive state, or
business rule. The assistant should clearly identify what it can assess
and what requires testing.

## License

No license has been specified yet. Add a `LICENSE` file before
presenting this repository as open source, and choose a license that
matches how you want others to use and modify the work.
