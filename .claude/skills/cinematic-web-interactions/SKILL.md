---
name: cinematic-web-interactions
description: Design or implement immersive, scroll-led website interactions with layered depth and clear user control. Use for cinematic landing pages, property tours, product stories, and scene transitions.
---

# Cinematic Web Interactions

Use a cinematic entrance or scroll-led scene when spatial continuity supports the story. This is a prototype recipe, not a universal pattern. Offer a clear way to skip, exit, or use a simpler version.

## Layered hero to interior

1. **Prepare depth layers.** Separate background from foreground subject (for example, sky and distant landscape behind buildings and water). Use transparency only where needed; check for seams at different sizes.
2. **Place type in the depth stack.** Position the headline between visual planes so foreground edges can overlap it. Keep text legible, selectable where practical, and responsive.
3. **Create reflection only when the surface supports it.** A flipped duplicate with reduced opacity, slight blur, and a fading mask can suggest reflected type on water. Match the image perspective and preserve contrast.
4. **Anchor the approach.** Make the hotspot a real button with an accessible name, keyboard access, visible focus, and a generous target. Calculate its position from the rendered image so the zoom origin tracks responsive crops.
5. **Transition scenes.** Move toward the hotspot, then reveal the interior with a short crossfade. The supplied walkthrough's 1.2-second zoom to about 6x and 400 ms crossfade are starting values; retune to the asset, device, and user preference.
6. **Map scroll to scene travel.** Divide each room segment into travel and a stable inspection period. The supplied 70% travel / 30% hold split is a starting point to test, not a law.
7. **Reveal titles during stable periods.** Keep essential reading still; fade titles in when the camera pauses. Make key information reachable without animation.
8. **Keep orientation and exit controls visible.** Show a subtle progress indicator and persistent return action. Do not trap visitors in a canvas or hijack normal scroll.

## Interaction and fallback

- Keep controls usable by keyboard, touch, assistive technology, zoom, and reduced-motion settings.
- Offer a skip or static-tour route; preserve browser back and ordinary page navigation.
- Provide meaningful fallback content if 3D, WebGL, video, or image assets fail or are unavailable.
- Do not make text or essential controls depend on one camera angle.
- Keep motion tied to user progress; avoid continuous movement while visitors read.
- Check loading, responsive crops, low-powered devices, focus management, and performance.
- For reduced motion, replace zoom and camera travel with direct scene changes or static room navigation.

Describe asset layers, stacking order, hotspot behavior, transition timeline, scroll mapping, title timing, persistent controls, fallback, and accessibility. For an audit, separate visible facts from implementation/device checks.

Use `web-design` for the full page and `motion-design` for other motion treatments.