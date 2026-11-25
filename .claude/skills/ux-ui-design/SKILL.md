---
name: ux-ui-design
description: Design or critique user experiences and interfaces for usability, clarity, accessibility, and task success. Use for product flows, screens, prototypes, and interaction patterns.
---

# UX/UI Design

Review the experience from the user's goal through the interface and its states. Use UX laws as prompts for questions, not rigid laws. Lists and names vary; validate recommendations against the task, audience, and evidence.

## Understand the task

Identify the user's goal, context, platform, constraints, and success/failure states. Inspect the full flow where possible: entry, choices, input, feedback, errors, completion, and recovery. With a screenshot alone, separate visible findings from behavioral assumptions.

## Useful UX lenses

- **Familiarity (Jakob's Law):** Familiar conventions reduce relearning. Depart when novelty benefits the task and the new pattern remains understandable.
- **Choice (Hick-Hyman Law):** Choice complexity affects decision effort. Group, label, filter, or sequence options where helpful; do not hide useful choices merely to reduce their number.
- **Targets (Fitts's Law):** Size, distance, placement, and input method affect target acquisition. Make important targets easy to reach, especially on touch.
- **Working memory:** Chunk information into meaningful groups and keep context visible. Treat “seven plus or minus two” as a shorthand, not a universal limit.
- **Gestalt grouping:** Proximity, similarity, common regions, continuity, and figure-ground affect how people parse interfaces. Make visual grouping match the information structure.
- **Feedback and time:** Give timely feedback for actions and waits. The often-cited 400 ms Doherty threshold is a heuristic, not a universal performance guarantee; measure the real experience.
- **Progress and completion:** Progress cues can help users resume meaningful tasks. Do not manufacture unfinished loops or pressure people to return.
- **Peak and end moments:** Pay attention to errors, confirmations, high-stakes steps, and exits as well as the average flow.
- **Simplicity and complexity:** Remove needless steps, but recognize that task complexity still exists. Decide what the system can safely handle and what users must understand.
- **Input tolerance:** Accept common harmless input variations when feasible, and give clear correction guidance.
- **Salience and sequence:** Emphasize the primary action without making everything compete. Test whether order helps people find and remember key items.

Behavior models can diagnose friction; do not use them to pressure users. Aesthetic polish can improve perceived usability, but cannot repair a broken or inaccessible interaction.

## Accessibility and states

Check keyboard use, visible focus, labels, contrast, target size, error identification, status announcements, zoom/reflow, and reduced motion as appropriate. Inspect default, hover, focus, pressed, disabled, loading, success, empty, and error states. Do not infer accessibility from a static image.

For each finding give **Location**, **Evidence**, **User impact**, **Recommendation**, and **Priority**. Separate confirmed issues from questions needing research or testing. Rank by task failure, user impact, frequency, and reach. Explain observed behavior rather than treating a named law as proof.

Use `design-foundations` for visual fundamentals and `web-design` for responsive web behavior.

Additional useful lenses include Law of Pragnanz and Occam's Razor (prefer the simplest interpretation or solution that still serves the task), Von Restorff (a distinct item can stand out, so reserve distinctiveness), and the Goal-Gradient and Zeigarnik effects (progress can support a real unfinished task without creating pressure). Parkinson's Law is a prompt to remove needless waiting and steps, not to impose arbitrary deadlines. Kano's model can distinguish expected basics, performance factors, and possible delights; validate which is which with users. The Fogg model frames behavior as motivation, ability, and a prompt; use it to lower task barriers, not to manipulate people.