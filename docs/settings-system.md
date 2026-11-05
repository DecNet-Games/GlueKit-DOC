---
layout: default
title: The Settings System
nav_order: 7
description: "Graphics, audio, gameplay and accessibility settings defined once as data, generated as working menus in both UGUI and UI Toolkit — same categories, same rows, same live model."
---

# The Settings System
{: .no_toc }

GlueKit's settings are **defined once, as data** — and generated as working menus in **both UGUI and UI Toolkit**. Same categories, same rows, same live model: a change made in one menu is the same change in the other, because both are views over one settings model, not two implementations that can drift.

## The four categories

- **Graphics** — quality and display settings, including the presets covered in [Graphics Presets & Display]({{ site.baseurl }}/docs/graphics-presets/).
- **Audio** — volume settings such as Music Volume and Master Volume, applied live through the settings model's event path (lowering Music Volume in the Playground is audible the moment you move the slider).
- **Gameplay** — your game's own options, declared alongside the built-in categories.
- **Accessibility** — the accessibility options category, defined in the same data as everything else.

## Restore Defaults, honestly scoped

**Restore Defaults** resets setting values to their defaults. It **never touches a player's key bindings** — settings reset and binding reset are separate actions by design, because a player who resets their graphics did not ask to lose their controls. See [Key Rebinding]({{ site.baseurl }}/docs/key-rebinding/) for its own Reset All Bindings action.

## Where it lives

The Home window's **Settings** section shows the active settings profile and the menu generation state. The menus themselves are runtime UI — they work in your built game, not only in the Editor.
