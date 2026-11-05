# PUSH NOTE — GlueKit-DOC (built 2026-11-05, local only, NOT pushed)

## What this folder is

The complete, push-ready source tree for GlueKit's documentation site, built to the Decnet house "-DOC" pattern (structure/config mirrored from MergeGuard-DOC / AgentProof-DOC / SteamDeck-DOC / ShipSheet-DOC):

- Just the Docs Jekyll site via `remote_theme` (no `theme:` gem key, no `just-the-docs` gem in the Gemfile — the pairing that fixed the two known GitHub Pages errors: "The just-the-docs theme could not be found" and "The github-pages gem can't satisfy your Gemfile's dependencies").
- 21 content pages: Home + Getting Started + Installation + Quick Start + The Home Window + One-Click Setup + The Settings System + Graphics Presets & Display + Key Rebinding + Save Slots + Autosave + Load Validation + The Debug Console + Console Commands + Stripping the Console from Release Builds + The Playground Sample + What v1 Is Not + FAQ + Troubleshooting + Changelog + Support.
- **No media in this tree, by design** (the MergeGuard-DOC precedent: zero screenshots, text-first documentation). GlueKit's Editor capture session has not run yet, and documentation never ships invented imagery: screenshots join `assets/` only after real captures exist, and the pages are written so they do not depend on any image.
- Content sourced ONLY from the verified record: the prep listing copy (`../../gluekit-prep/LISTING-COPY.md` — every capability line is one of its SPEC-13 allowed claims) and the build evidence in `~/workspace/laptop-runs/gluekit-work/GAP-REPORT.md` (47/47 EditMode on Unity 6 in the development and clean projects; Playground five-action self-tests passing in development, release and clean-project Windows players; G-FINAL GO). **Binding fences held everywhere:** Unity 6 ONLY — 2022.3 support is never implied; the save leg is documented as slots / autosave / load validation only — no migration, cloud sync, corruption recovery, backup, encryption or tamper claims; platform verification is stated as Unity 6 Editor + Windows PC players only (no console/mobile/WebGL claim).
- No product Asset Store URL exists yet (no portal draft for GlueKit has been created — draft creation follows the capture stage), so Home/Installation link the Decnet Games publisher page (118262) — swap in the product URL after the listing goes live, as with the other -DOC trees.

## Exact repo to create

- **Name:** `GlueKit-DOC`
- **Owner:** `DecNet-Games` (GitHub org account)
- **Visibility:** public (required for GitHub Pages on this setup)
- **Live URL once Pages is on:** https://decnet-games.github.io/GlueKit-DOC/ (matches the `baseurl: "/GlueKit-DOC"` already set in `_config.yml`)

## Push route (do this from the laptop, per the standing no-card-spam rule)

Bulk pushes go via laptop git over SSH — never the GitHub connector.

1. BOSS creates the empty repo `DecNet-Games/GlueKit-DOC` on GitHub (no README, no .gitignore — this tree is the repo content).
2. Copy this folder's contents to the laptop clone location, then: `git init` (if needed) → `git add .` → `git commit` → the final `git push` is BOSS's own ~10-second action at his terminal (laptop git credentials only work interactively — known constraint).
3. On GitHub: repo **Settings → Pages → Build and deployment → Source: GitHub Actions** (the standard github-pages workflow), or "Deploy from a branch" → `main` / root if Actions is unavailable. The other -DOC repos run on the same org setup — mirror whichever source they use.
4. After the first successful build, verify:
   - the live URL loads with the Just the Docs theme (no theme error),
   - nav order: Home, Getting Started, Installation, Quick Start, The Home Window, One-Click Setup, The Settings System, Graphics Presets & Display, Key Rebinding, Save Slots, Autosave, Load Validation, The Debug Console, Console Commands, Stripping the Console from Release Builds, The Playground Sample, What v1 Is Not, FAQ, Troubleshooting, Changelog, Support.
5. Only after the site is live: apply the house-format description (`../DESCRIPTION-HOUSE.md`) to GlueKit's portal draft once that draft exists — its link line carries `DOCUMENTATION → https://decnet-games.github.io/GlueKit-DOC/` (dead-link rule: never publish the link before the site resolves).

## What remains

- Repo creation + push + Pages enable: BOSS-side steps above (by design — this build stopped at a complete local tree, per instructions).
- Media: after GlueKit's Editor capture session runs, real frames land in `../raw/` and can be added under `assets/images/` with a small content update — not required for the site to be complete or correct.
- Portal draft: not yet created for GlueKit (it follows the capture stage in the pipeline); the plain portal text is `../../gluekit-prep/LISTING-COPY.md`, and `../DESCRIPTION-HOUSE.md` is the prepared house-format replacement for when the site is live.
- Nothing in the tree itself: content, config and Gemfile are complete and internally verified (page count, front matter, nav order checked against disk).
