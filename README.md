# Productivity Paradox Slidev Deck

Slidev deck for a 10-15 minute internal knowledge-sharing talk on Paul A. David's 1990 essay, *The Dynamo and the Computer*, with a cautious extension to AI adoption.

The core idea:

> Productivity payoff often comes less from bolting a new tool onto an old system, and more from redesigning the system around the new tool.

## Talk Shape

The deck uses electrification as a historical mirror for the computer productivity paradox, then uses both as a frame for thinking about AI.

Main arc:

1. Robert Solow's productivity-paradox quote: computers were visible everywhere except in the productivity statistics.
2. David's comparison: early computers around 1990 looked like early factory electrification around 1900.
3. Adoption came first; measured payoff came later.
4. The mechanism was redesign: factories had to move from central group drive and line shafts to unit drive and workflow-oriented layouts.
5. Computers later showed a delayed payoff, especially in the 1995-2004 productivity acceleration, but the payoff was not permanent or automatic.
6. AI is treated as an observation frame, not a forecast: are we merely adding AI to old workflows, or redesigning work around it?

The presentation keeps the main path simple and pushes caveats, source disputes, and extra examples into backup slides and notes.

## Repository Layout

```text
slides.md      Main Slidev deck, including slide markup and speaker notes.
style.css      Shared deck styling.
assets/        Images, diagrams, and generated chart SVGs used by the deck.
data/          Small CSV sources behind the electrification and TFP charts.
notes/         Source notes, fact checks, background reading, and scripts.
DEPLOYMENT.md  Cloudflare Pages + GitHub Actions deployment instructions.
```

Important supporting files:

```text
notes/source-notes.md
notes/speaker-script.md
notes/speaker-script-10min.md
notes/speaker-script-10min.zh.md
notes/speaker-script-spoken.zh.md
notes/background-industrial-revolutions.md
notes/background-industrial-revolutions.zh.md
notes/group-drive-unit-drive-fact-check.md
notes/electrification-1920s-tfp-attribution.md
notes/early-tfp-growth-not-electrification.md
```

## Local Development

Install dependencies:

```bash
npm install
```

Start the Slidev dev server:

```bash
npm run dev
```

Open the normal presentation view:

```text
http://localhost:3030/1
```

Navigate with the arrow keys. Use `?print` only for print/export-style checks, not for presenting.

## Build

Build the static site:

```bash
npm run build
```

The generated site is written to `dist/`. This directory is ignored by git.

Export with Slidev:

```bash
npm run export
```

## Deployment

The intended deployment target is Cloudflare Pages, using GitHub Actions to build the deck and upload `dist/` with Wrangler.

See [DEPLOYMENT.md](DEPLOYMENT.md) for the full setup, including:

- Cloudflare Pages project creation
- Cloudflare API token permissions
- GitHub Actions repository secrets
- manual and automatic deployment paths

The deployment workflow is:

```text
.github/workflows/deploy-cloudflare-pages.yml
```

## Public Sharing Note

The deployed site is public. The current project is intended to contain public/shareable material only, but review `slides.md`, `assets/`, and `notes/` before publishing anything new.

This repo currently uses Slidev `0.50.0`. Plain `slidev build` works. The newer `--without-notes` option mentioned in current Slidev docs is not supported by this installed version.

## Editing Guidance

When editing the talk:

- Keep the main deck light enough for a 10-15 minute sharing session.
- Put detailed evidence, disputes, and caveats in backup slides or `notes/`.
- Treat the AI section as a framing analogy, not a hard prediction.
- Preserve the distinction between adoption, diffusion, redesign, and measured productivity.
- When adding quantitative claims, add the source or caveat to `notes/source-notes.md`.

## Current Draft Principle

Keep it simple: no fancy animation, no dense econ math. The audience should leave with one transferable mechanism:

```text
new tool + old workflow = limited payoff
new tool + redesigned workflow = possible productivity payoff
```
