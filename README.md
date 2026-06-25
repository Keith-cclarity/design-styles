# design-styles

A Claude skill: a working library of **50 named design styles** (Neoclassical, Synthwave, Neo-Brutalism, Japandi, Glassmorphism, and more) for steering aesthetic direction across carousels, videos, images, and frontend builds.

Naming a style up front ("Ethereal UI", "Neo-Brutalist layout") instantly narrows any AI output and lets you brief precisely instead of describing a vibe.

## What's inside

- **`SKILL.md`** — the skill entry point: when to use it, the method, and a worked example.
- **`CATALOGUE.md`** — all 50 styles. Each entry has a reference image, description, core elements, mood & occasion, type / layout / motion notes, starter CSS tokens, and a ready-to-adapt AI prompt scaffold.
- **`references/images/`** — 50 reference images, one per style. View them to *see* the style, not just read it.
- **`references/styles.json`** — structured data (name, slug, description, core, mood) for programmatic use.

## Use it for

- Trying a specific named aesthetic on a piece of content
- Building a fast moodboard of 3-4 candidate directions
- Mixing two styles into a hybrid (e.g. *Vaporwave × Gothic*)
- Writing a sharper AI image/video generation prompt

## Install

Drop the `design-styles/` folder into your Claude skills directory (e.g. `~/.claude/skills/design-styles/`), then invoke it with `/design-styles` or let it trigger on a named style.

## Credit

Style names, descriptions, core elements, and mood are adapted from *50 Design Styles Every Designer Should Know for Better Prompting* by Himanshu Bhardwaj (UX Planet). Prompt scaffolds and starter CSS tokens are additions for AI-generation and frontend workflows.
