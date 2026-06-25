---
name: design-styles
description: A library of 50 named design styles (Neoclassical, Synthwave, Neo-Brutalism, Japandi, Glassmorphism, etc.) for experimenting with aesthetic direction across carousels, videos, images, and frontend builds. Each style has a description, core elements, mood, a saved reference image, an AI image/video prompt scaffold, and starter CSS tokens. Use when the user wants to try a specific named aesthetic, explore design directions, build a moodboard, mix two styles into a hybrid, or write a better AI generation prompt. Triggers on a named style ("make this carousel Synthwave", "Japandi version"), "design style", "try a different aesthetic", "moodboard", or browsing directions for a brand/content piece.
---

# Design Styles

A working library of **50 named design styles** for experimenting with aesthetic direction. Built from *50 Design Styles Every Designer Should Know for Better Prompting* (Himanshu Bhardwaj, UX Planet), extended with prompt scaffolds and starter CSS tokens for AI generation and frontend work.

The point: **style fluency**. Naming a style up front ("Ethereal UI", "Neo-Brutalist layout") instantly narrows any AI output and lets you brief precisely instead of describing a vibe.

## Files

- **`CATALOGUE.md`** — all 50 styles. Each entry: reference image, description, core elements, mood & occasion, type direction, layout & motion notes, starter CSS tokens, and a ready-to-adapt AI prompt scaffold.
- **`references/images/NN-slug.png`** — 50 saved reference images (one per style). View these to SEE the style, not just read it.
- **`references/styles.json`** — structured data (name, slug, description, core, mood) for programmatic use.

## How to use it

**1. Pick or get given a style.** If the user names one ("make it Art Deco"), go straight to that entry in `CATALOGUE.md` and open its reference image. If they're exploring, show 3-4 candidate styles for the same concept (a fast moodboard) so they can choose — visual clarity = decision clarity.

**2. For AI image/video generation** (Higgsfield, GPT Image, HyperFrames visuals): start the prompt with the style name, then paste the entry's **prompt scaffold** and fill the brackets with the real subject, composition, lighting, medium, and aspect ratio. Reference image can be used as a visual reference where the tool supports it.

**3. For carousels / decks / frontend builds:** lift the entry's **starter tokens** and **type / layout / motion** notes as the project's base brand system, then adapt. Tokens are a STARTING POINT — tune them for contrast and hierarchy, don't ship them raw.

**4. Mix styles for a hybrid.** Once you know each style's DNA, combine two: "Vaporwave x Gothic", "Luxury Typography meets Aurora", "Japandi x Neo-Brutalism". State both names and blend their core elements + palettes.

**5. Brief precisely.** "Make it feel like Art Nouveau meets Kawaii" communicates faster to any tool or collaborator than describing the feeling.

## Worked example

Say the brief is a hero image for a meditation app, and Aurora is chosen.

**Open the entry**, read its core elements and mood, and look at `references/images/03-aurora.png` to confirm the feel.

**Fill the prompt scaffold** (replace the brackets with the real subject and shot details):

> A lone figure seated cross-legged on a still lake at dawn, in the **Aurora** style. Iridescent gradients, blur effects, soft glows, translucent overlays, organic wave forms. Mood: dreamy, futuristic, meditative. Suitable for wellness apps. Wide cinematic composition, low-key ambient light, soft-focus photographic medium, 16:9.

A good result reads unmistakably as Aurora — iridescent teal/violet drift, glow, weightlessness — not a generic gradient. If you could swap the style name out and the image wouldn't change, the style cues were too weak.

**Lift the tokens** for a matching landing section, then ADAPT (these are the entry's starting values, tuned for contrast):

```css
:root { --bg:#0B1026; --teal:#5EEAD4; --violet:#A78BFA; --pink:#F472B6; --text:#E6E8F2; }
/* tuned: darkened bg for AA text contrast, violet reserved for one accent only */
```

The image and the section now share one palette and one mood — that consistency is the whole point.

## Important notes

- **Starter tokens are starting points, not rules.** They're credible defaults to adapt per piece, not a fixed spec.
- **This skill supplies aesthetic *direction*, not a finished design.** The usual design process still applies for real builds — user journey, information hierarchy, restraint, accessibility. A style name is the starting brief, not the whole job.
- **An existing brand system takes precedence.** If the project already has a brand guide, honour it. Reach for these styles when the surface is greenfield, exploratory, or client work without a fixed identity, or as raw material when deliberately revamping a direction.

## The 50 styles

1. Neoclassical · 2. Baroque · 3. Aurora · 4. Ethereal · 5. Filigree · 6. Acanthus · 7. Anthropomorphic · 8. Pixel Art · 9. Conceptual Sketch · 10. Luxury Typography · 11. Japandi · 12. Memphis · 13. Bohemian · 14. Shabby Chic · 15. Farmhouse / Cottagecore · 16. Victorian · 17. Art Deco · 18. Art Nouveau · 19. Mystical Western · 20. Kitsch · 21. Y2K · 22. Bauhaus · 23. Brutalism · 24. Cybercore · 25. Synthwave · 26. Vaporwave · 27. Pop Art · 28. Bento Box · 29. Graffiti · 30. Tenebrism · 31. Gothic · 32. Pointillism · 33. Mixed Media · 34. Steampunk · 35. Kawaii · 36. Coquette · 37. Surrealism · 38. Utilitarian · 39. Mid-Century · 40. Scrapbook · 41. Neo Frutiger Aero · 42. Dark Magic Academia · 43. Light Academia · 44. Wabi Sabi · 45. South West / Wild West · 46. Nautical · 47. Rebus · 48. Glassmorphism · 49. Modular Typography · 50. Neo-Brutalism

Full detail + reference image for each in **`CATALOGUE.md`**.
