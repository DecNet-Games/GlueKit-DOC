---
layout: default
title: Graphics Presets & Display
nav_order: 8
description: "Presets that are not quality labels: each preset drives your URP or HDRP Volume profile as well as the quality level, at runtime, without a scene reload. Resolution changes use keep-or-revert confirmation."
---

# Graphics Presets & Display
{: .no_toc }

## Presets that do something

A GlueKit graphics preset is not a quality label. Each preset drives **your URP or HDRP Volume profile** as well as the **quality level** — so "High" means your post-processing changes with it, not just a number in a list. Switching presets takes effect **at runtime, without a scene reload**.

## Display changes confirm themselves

Resolution and fullscreen changes use the confirmation players expect: the change applies, a **keep-or-revert countdown** runs, and if the player does not confirm — because the new mode left them looking at a screen they cannot use — the previous mode comes back on its own. A settings menu should never be able to strand a player on an unusable display mode.

## Part of one model

Presets and display settings live in the same settings data as every other category — see [The Settings System]({{ site.baseurl }}/docs/settings-system/). Restore Defaults resets these values without touching key bindings.
