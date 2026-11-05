---
layout: default
title: Load Validation
nav_order: 12
description: "Before a save can be loaded it is validated. A save that cannot be read, or that a newer game version made, is shown as unavailable with the reason in plain language — never loaded over the player's progress."
---

# Load Validation
{: .no_toc }

A save slot is a promise. Before any GlueKit save can be loaded, it is **validated** — because the worst thing a save system can do is load something broken over the top of a player's progress and call it fine.

## What validation catches

- **A save that cannot be read** — the data is not loadable in its current state.
- **A save a newer game version made** — the slot's recorded game version is ahead of the build trying to load it.

## What the player sees

A save that fails validation is shown as **unavailable, with the reason in plain language** — not a greyed-out mystery, not an exception, and never a silent load attempt. The player keeps their other slots and their progress; the bad slot is named and explained.

## What validation is not

Validation is a **check before loading**, not a repair service. GlueKit does not claim corruption recovery, save migration between versions, or backup restoration — the boundary is stated in [What v1 Is Not]({{ site.baseurl }}/docs/what-v1-is-not/) and in the package's own copy of that page.
