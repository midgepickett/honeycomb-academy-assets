# Honeycomb Academy — Brand & Asset Repo

## What this repo is
Brand assets, design instructions, and a Claude Code skill for generating
on-brand content — comics, slides, diagrams, and components.

## Structure
- `assets/` — all brand PNG assets
- `.claude/SKILL.md` — brand guidelines, asset URLs, and behavioral
  instructions. Claude Code reads this automatically on startup.
- `components/` — reusable HTML templates (generated)
- `output/` — generated content files

## Asset URLs
All assets served via jsDelivr:
`https://cdn.jsdelivr.net/gh/midgepickett/honeycomb-academy-assets@main/assets/`

## Using Claude Code
1. Clone this repo
2. Install Claude Code: `brew install --cask claude-code`
3. Run `claude` from the repo root — SKILL.md loads automatically
4. Describe what you want — Claude applies the full brand

## Adding new assets
1. Drop the PNG into the `assets/` folder
2. Push to main
3. Add the jsDelivr URL and usage note to `.claude/SKILL.md`