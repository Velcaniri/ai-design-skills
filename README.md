# Product Page UX Audit

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Status: Active](https://img.shields.io/badge/status-active-brightgreen.svg)](#)
[![Skill](https://img.shields.io/badge/type-AI%20Skill-purple.svg)](skill.md)

A reusable AI skill for auditing e-commerce product pages, identifying UX/UI problems, and turning design feedback into clear, prioritized, actionable recommendations.

> Great product-page design is more than visual polish. It helps shoppers understand a product, evaluate it, trust the information, and purchase with confidence.

## Contents

- [Overview](#overview)
- [What it checks](#what-it-checks)
- [How to use the skill](#how-to-use-the-skill)
- [Example prompts](#example-prompts)
- [Repository structure](#repository-structure)
- [How audits are structured](#how-audits-are-structured)
- [Design principles](#design-principles)
- [Limitations](#limitations)
- [Contributing](#contributing)
- [License](#license)

## Overview

**Product Page UX Audit** gives an AI assistant a repeatable framework for reviewing e-commerce product detail pages. It can be used with screenshots, mockups, prototypes, or implemented pages.

The skill includes a checklist of 15 common product-page problems, three optional UX enhancements, and a workflow for turning observations into prioritized fixes.

It is designed to encourage specific, evidence-based feedback—not vague comments like "make it cleaner" or arbitrary redesign suggestions.

## What it checks

The audit checklist covers:

| # | Area | What to look for |
|---:|---|---|
| 1 | Image contrast | Navigation icons that disappear against product imagery |
| 2 | Product imagery | Weak focal points, misleading images, inconsistent catalog styling |
| 3 | Alignment | Elements that do not follow a consistent layout grid |
| 4 | Color | Overly saturated colors and competing emphasis |
| 5 | Typography | Inconsistent font families, weights, and hierarchy |
| 6 | Labels and badges | Cramped labels and overloaded discount badges |
| 7 | Product title | Weak or unbalanced title hierarchy |
| 8 | Description | Difficult-to-read body text and line spacing |
| 9 | Reviews | Ratings and review information detached from the title |
| 10 | Feature icons | Inconsistent icon styles, weights, and colors |
| 11 | Dividers | Heavy separators that fragment the page |
| 12 | Spacing | Gaps that disconnect related content or crowd sections |
| 13 | Price labels | Redundant labels that add no useful information |
| 14 | Quantity and price | Confusing units, quantities, and total-price presentation |
| 15 | Purchase action | Poorly grouped quantity controls and add-to-cart actions |

### Additional UX enhancements

The skill also considers three optional patterns when they suit the product and platform:

- **Scrollable product-details card** — separates product imagery and details while preserving context.
- **Sticky purchase area** — keeps key purchase controls accessible during longer scrolls.
- **Predefined quantity options** — offers convenient one-tap choices while preserving custom selection where needed.

These are not universal rules. The skill asks the assistant to explain the user benefit and trade-offs before recommending them.

## How to use the skill

1. Open [`skill.md`](skill.md).
2. Copy or download the skill instructions.
3. Add the file to the skills directory or import it using the skill-loading process supported by your AI tool.
4. Give the assistant a product-page screenshot, mockup, prototype, or page to review.
5. Ask for an audit or redesign plan.

Installation paths differ between AI tools, so follow the instructions for your specific platform.

## Example prompts

Try prompts such as:

- "Audit this product page and identify its biggest UX problems."
- "Review this e-commerce screenshot. Focus on alignment, hierarchy, spacing, and typography."
- "Find usability problems in this product detail page and prioritize the fixes."
- "Critique this redesign. Which changes genuinely improve the shopping experience?"
- "Create a practical redesign plan for this product page."

## Repository structure

```text
product-page-ux-audit/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.md
│   │   └── feature_request.md
│   └── PULL_REQUEST_TEMPLATE.md
├── examples/
│   └── audit-template.md
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── README.md
├── SECURITY.md
└── skill.md
```

## How audits are structured

The skill encourages an audit to include:

- **Overall assessment** — a concise summary of the page's strengths and weaknesses.
- **Findings** — the affected area, problem, user impact, and recommended correction.
- **Priority** — Critical, High, Medium, or Low, with a reason.
- **Recommended fix order** — the highest-impact changes first.
- **Optional enhancements** — improvements that are useful but not required to fix a defect.
- **Verification notes** — anything that cannot be confirmed from the supplied material.

The checklist is a diagnostic reference, not a quota. The assistant should report only issues that are actually present.

## Design principles

- Design for a reusable product system, not one screenshot.
- Prioritize clarity over decoration.
- Make product identity, ratings, pricing, options, and purchase actions easy to find.
- Keep related controls together.
- Make units, selected quantities, and totals understandable.
- Use consistent typography, spacing, alignment, color, and iconography.
- Explain the user impact behind every recommendation.
- Distinguish objective usability problems from personal visual preferences.

## Limitations

This skill is a design-review aid, not a replacement for user research or usability testing.

A screenshot can reveal many visual issues, but it cannot confirm every interaction, responsive state, accessibility behavior, or business rule. The assistant should clearly distinguish what is visible from what needs further inspection or testing.

## Contributing

Suggestions, improvements, and corrections are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening an issue or pull request.

## License

This project is licensed under the [MIT License](LICENSE).
