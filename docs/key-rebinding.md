---
layout: default
title: Key Rebinding
nav_order: 9
description: "Rebinding on Unity's Input System: per-action panels in both menu stacks, per-scheme bindings, device glyphs with text fallback, and conflicts resolved with Swap, Replace, or Cancel — never a silent steal."
---

# Key Rebinding
{: .no_toc }

GlueKit's rebinding is built on **Unity's Input System** — the one your project already uses. Projects on the legacy Input Manager are not supported in v1.

## You choose what is rebindable

You designate which actions players may rebind. Players get a per-action rebind panel, present in **both menu stacks** (UGUI and UI Toolkit), with **per-scheme bindings**: a keyboard binding and a gamepad binding for the same action are separate rows, each shown with its **device glyph** — and an automatic **text fallback** when no glyph exists for a device.

## Conflicts are handled, not hidden

Capture a key another action already uses and the panel **names the conflict** and offers three outcomes:

- **Swap** — the two actions exchange bindings.
- **Replace** — the captured key moves to this action, and the other action is left for the player to resolve.
- **Cancel** — nothing changes.

A binding is **never silently stolen**, and a required action is never left unbound without being flagged. Overrides **persist across sessions**, so a player's controls are still their controls next launch.

## Reset belongs to the player, separately

**Reset All Bindings** is its own action, separate from the settings system's Restore Defaults — resetting graphics never wipes controls, and resetting controls never wipes settings values. The Home window's Input Rebinding section shows the rebind profile and binding counts.
