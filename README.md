# Product Page UX Audit and Design Skills

A collection of portable Agent Skills for auditing product pages and designing graphics, interfaces, websites, and motion. The original e-commerce product-page audit remains available alongside focused skills.

## Skill library

| Skill | Use it for |
|---|---|
| [Product Page UX Audit](.agents/skills/product-page-ux-audit/SKILL.md) | E-commerce product detail page reviews and prioritized fixes |
| [Design Foundations](.agents/skills/design-foundations/SKILL.md) | Shared visual principles across disciplines |
| [Graphic Design](.agents/skills/graphic-design/SKILL.md) | Posters, social graphics, ads, editorial layouts, and visual assets |
| [UX/UI Design](.agents/skills/ux-ui-design/SKILL.md) | Usability, interaction flows, interface screens, and prototypes |
| [Web Design](.agents/skills/web-design/SKILL.md) | Responsive websites, page structure, and web-specific review |
| [Motion Design](.agents/skills/motion-design/SKILL.md) | Animation concepts, style choices, timing, and motion critique |
| [Cinematic Web Interactions](.agents/skills/cinematic-web-interactions/SKILL.md) | Layered hero scenes, anchored zooms, and scroll-led tours |

Each skill has a matching copy under `.claude/skills/`. The instructions are platform-neutral and use the Agent Skills folder format. They are intended for AI products that support this skills format or can import it. Products without a skills feature are outside the supported use case; import steps and compatibility vary by product and version.

## Shared quality bar

- Start from the audience, purpose, task, and constraints.
- Treat design principles and UX laws as context-sensitive heuristics, not commandments.
- Base critiques on observable evidence; mark assumptions and unverified behavior.
- Explain the user or communication impact, give a concrete recommendation, and prioritize it.
- Keep accessibility, responsive behavior, and appropriate user control in view.
- Separate necessary fixes from optional polish.

## Installation

Choose the skill directory that matches the importing product's documented Agent Skills workflow. Products may discover project skills under `.agents/skills/<skill-name>/SKILL.md` or `.claude/skills/<skill-name>/SKILL.md`. Keep the folder name aligned with the YAML frontmatter `name`, then follow that product's documented refresh or activation step. If a product uses another skill format, adapt the content to that format.

The root `skill.md` remains a convenient copy of the original product-page audit.

## References

The skills synthesize, in original wording, the six supplied design-principle articles and the two supplied video descriptions. The articles vary in how they name and count principles; the skills preserve overlapping ideas and avoid treating any list as universal. Video timings are examples to prototype and tune.

- [Medium: 12 Laws of UX](https://medium.com/uxness/12-laws-of-ux-designing-with-principles-for-user-delight-23166f687704)
- [My UX Academy: UX Design Laws and Principles](https://myuxacademy.com/blog/ux-design-laws-principles/)
- [Maze: The 21 Main UX Laws](https://maze.co/collections/ux-ui-design/ux-laws/)
- [Adobe Express: 8 Basic Design Principles](https://www.adobe.com/express/learn/blog/8-basic-design-principles-to-help-you-create-better-graphics)
- [Toptal: 12 Principles of Design](https://www.toptal.com/designers/ui/principles-of-design)
- [Figma: 13 Graphic Design Principles](https://www.figma.com/resource-library/graphic-design-principles/)

## Limitations

These skills support design critique and planning; they do not replace user research, usability tests, accessibility evaluation, or real-device checks. A screenshot cannot confirm behavior that is not visible.

## License

This project is licensed under the [MIT License](LICENSE).
