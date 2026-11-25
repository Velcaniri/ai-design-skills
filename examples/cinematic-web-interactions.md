# Example: Cinematic Web Interactions

## Scenario

A lakeside home listing uses a cinematic hero to invite visitors into a room-by-room tour.

## Interaction outline

1. Use a distant landscape as the back plane and the home and lake as the foreground plane.
2. Place the property name between the two planes so the roofline overlaps the letters.
3. Add a subtle reflected version of the title only if it fits the water perspective and remains legible.
4. Make a visible lantern hotspot a keyboard-accessible button.
5. On activation, zoom toward the lantern and transition to the interior scene.
6. Link scroll progress to room-to-room travel, then pause the camera so visitors can inspect each room and read its title.
7. Keep a progress indicator and “Back to the lake” control available throughout.

## Review checks

Try the flow with keyboard, touch, reduced motion, narrow screens, slow loading, and WebGL unavailable. Preserve ordinary browser back and scroll behavior. The room information must remain reachable in a static or simplified tour.

Any zoom scale, transition duration, or travel/hold ratio should be tuned with the actual imagery and tested on devices; sample values are not design laws.