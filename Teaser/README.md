# Teaser

This folder contains the NOEME teaser assets.

The teaser presents the NOEME / PROTOTYPE intro through two faces, timed fades, letter animation, blur, and glow.

NOEME appears first, letter by letter. PROTOTYPE follows after, building from the center outward.

During the disappearance, PROTOTYPE breaks first. Letters vanish from its outermost positions. Each paired disappearance lights a letter in NOEME, gradually spelling “ONE ME” backwards until only the left O remains.

As the “ONE ME” reading becomes visible, one of the eyes turns pale. This connects the title animation back to the visual language of the Condition.

The final O from PROTOTYPE falls into the O of NOEME. Once the two O letters meet, NOEME begins disappearing letter by letter, now spelling “ONE ME” forward.

## Animation Design

The teaser was built in HTML/CSS rather than assembled only as a static video. The sequence uses individually timed letter animations, opacity transitions, blur effects, glow states, and eye-state changes.

Small timing adjustments, often between 0.01 and 0.2 seconds, were used to synchronize the disappearance of PROTOTYPE, the emergence of “ONE ME,” the pale-eye transition, and the final convergence of the O letters.

`Teaser HTML.md` contains the implementation and timing code used to build the animation.

`Teaser.gif` is used for quick viewing inside GitHub.

`Teaser.mp4` is the full playback version.

---
© Diogo Oliveira — June 2026
