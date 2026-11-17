# Product Page UX Audit

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Agent Skill](https://img.shields.io/badge/format-Agent%20Skills-purple.svg)](https://agentskills.io/)
[![Platforms](https://img.shields.io/badge/platforms-Claude%20%7C%20Codex%20%7C%20more-5865F2.svg)](#platform-compatibility)

A reusable AI skill for auditing e-commerce product pages, identifying UX/UI problems, and turning design feedback into clear, prioritized, actionable recommendations.

> Great product-page design is more than visual polish. It helps shoppers understand a product, evaluate it, trust the information, and purchase with confidence.

## Contents

- [Overview](#overview)
- [What it checks](#what-it-checks)
- [Platform compatibility](#platform-compatibility)
- [Installation](#installation)
  - [Codex](#codex)
  - [Claude Code](#claude-code)
  - [Claude.ai](#claudeai)
  - [Other Agent Skills-compatible tools](#other-agent-skills-compatible-tools)
- [Using the skill](#using-the-skill)
- [Example prompts](#example-prompts)
- [Repository structure](#repository-structure)
- [Limitations](#limitations)
- [Contributing](#contributing)
- [License](#license)

## Overview

**Product Page UX Audit** gives an AI assistant a repeatable framework for reviewing e-commerce product detail pages. It can be used with screenshots, mockups, prototypes, or implemented pages.

The skill includes a checklist of 15 common product-page problems, three optional UX enhancements, and a workflow for turning observations into prioritized fixes.

It encourages specific, evidence-based feedback—not vague comments like "make it cleaner" or arbitrary redesign suggestions.

## What it checks

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

- **Scrollable product-details card** — separates product imagery and details while preserving context.
- **Sticky purchase area** — keeps key purchase controls accessible during longer scrolls.
- **Predefined quantity options** — offers convenient one-tap choices while preserving custom selection where needed.

These are optional patterns, not universal rules. The skill asks the assistant to explain user benefits and trade-offs before recommending them.

## Platform compatibility

The skill uses the open Agent Skills folder format: a skill directory containing a `SKILL.md` file with YAML frontmatter (`name` and `description`) followed by instructions.

| Platform | Supported setup |
|---|---|
| OpenAI Codex | Project or personal skill directory |
| Claude Code | Project or personal skill directory |
| Claude.ai | Upload the skill folder as a ZIP through the Skills settings |
| Other compatible agents | Use the platform's documented Agent Skills directory or import workflow |

Availability and exact setup can vary by product, version, and account.

## Installation

### Codex

**Option A — install from this GitHub repository**

In Codex, invoke the built-in `$skill-installer` and ask it to install this repository's skill from:

`https://github.com/Velcaniri/product-page-ux-audit/tree/main/.agents/skills/product-page-ux-audit`

**Option B — install manually**

Copy the `product-page-ux-audit` skill folder into one of these locations:

- **Project:** `.agents/skills/product-page-ux-audit/SKILL.md` inside your repository.
- **Personal:** `~/.agents/skills/product-page-ux-audit/SKILL.md`.

On Windows, `~` refers to your user profile directory. Restart Codex if the skill does not appear.

### Claude Code

Copy the `product-page-ux-audit` folder into either:

- **Project:** `.claude/skills/product-page-ux-audit/SKILL.md` inside your project.
- **Personal:** `~/.claude/skills/product-page-ux-audit/SKILL.md`.

Claude Code discovers skills from these directories. Use the skill by asking Claude Code to audit a product page, or explicitly invoke it using the skill name if your interface supports that workflow.

### Claude.ai

Claude.ai accepts custom skills as ZIP uploads on supported plans with the required features enabled.

1. Download or copy the `product-page-ux-audit` folder from this repository.
2. Make sure the folder contains `SKILL.md` directly inside it.
3. ZIP the folder itself. The ZIP should contain the folder, not just loose files.

   Correct:
   ```text
   product-page-ux-audit.zip
   └── product-page-ux-audit/
       └── SKILL.md
   ```

4. In Claude, open **Customize → Skills** (the exact menu may vary).
5. Upload the ZIP and enable the skill.

### Other Agent Skills-compatible tools

For tools that support the Agent Skills format:

1. Download the `SKILL.md` from `.agents/skills/product-page-ux-audit/`.
2. Put it in the skill directory documented by that tool.
3. Keep the folder name and frontmatter `name` aligned.
4. Follow the tool's instructions for refreshing or enabling newly added skills.

Not every AI assistant supports the same skill format. If a tool does not support Agent Skills, provide `SKILL.md` as context or adapt it to that tool's own custom-instructions feature.

## Using the skill

Once installed, provide a product-page screenshot, mockup, prototype, or page and ask for an audit or redesign plan. The assistant should:

1. Understand the product, audience, platform, and shopping context where available.
2. Inspect hierarchy, imagery, information, controls, and purchase flow.
3. Identify issues that are actually present.
4. Explain each issue and its impact on the user.
5. Recommend a concrete correction.
6. Prioritize findings by severity.
7. Separate necessary fixes from optional enhancements.
8. Identify anything that needs further testing or cannot be verified.

The checklist is a diagnostic reference, not a quota. The assistant should not invent problems to reach a certain number of findings.

## Example prompts

- "Audit this product page and identify its biggest UX problems."
- "Review this e-commerce screenshot. Focus on alignment, hierarchy, spacing, and typography."
- "Find usability problems in this product detail page and prioritize the fixes."
- "Critique this redesign. Which changes genuinely improve the shopping experience?"
- "Create a practical redesign plan for this product page."

## Repository structure

```text
product-page-ux-audit/
├── .agents/
│   └── skills/
│       └── product-page-ux-audit/
│           └── SKILL.md
├── .claude/
│   └── skills/
│       └── product-page-ux-audit/
│           └── SKILL.md
├── .github/
│   ├── ISSUE_TEMPLATE/
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

The root-level `skill.md` is retained as a convenient reading/download copy. The platform-ready copies use the conventional `SKILL.md` filename inside their respective skill directories.

## Limitations

This skill is a design-review aid, not a replacement for user research or usability testing. A screenshot can reveal many visual issues, but it cannot confirm every interaction, responsive state, accessibility behavior, or business rule. The assistant should distinguish what is visible from what needs further inspection or testing.

## Contributing

Suggestions, improvements, and corrections are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening an issue or pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Official platform documentation

- [OpenAI — Build skills](https://learn.chatgpt.com/docs/build-skills)
- [Anthropic — Create custom Skills](https://support.claude.com/en/articles/12512198-how-to-create-custom-skills)
- [Anthropic — Agent Skills overview](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview)
- [Agent Skills open format](https://agentskills.io/)
