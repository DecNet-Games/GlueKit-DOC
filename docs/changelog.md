---
layout: default
title: Changelog
nav_order: 20
description: "GlueKit 1.0.0 — the initial release: the settings system, Input System rebinding, save slots with autosave and load validation, and the extensible debug console, plus the Playground sample."
---

# Changelog
{: .no_toc }

## 1.0.0 — initial release

- GlueKit Home — one Editor window: Welcome with one-click setup and verification, Leg Status for all four systems, and sections for Settings, Input Rebinding, Save Slots, Debug Console, and Samples.
- Settings system: graphics, audio, gameplay and accessibility categories defined once as data, generated as menus in both UGUI and UI Toolkit on one live model; graphics presets driving URP and HDRP Volume profiles plus quality level at runtime; resolution/fullscreen keep-or-revert confirmation; Restore Defaults that never touches key bindings.
- Input rebinding on Unity's Input System: per-scheme bindings in both menu stacks, keyboard and gamepad glyphs with text fallback, conflict handling with Swap / Replace / Cancel, persistent overrides, and a separate Reset All Bindings action.
- Save slots: five manual slots plus a dedicated autosave slot manual saves cannot overwrite; slot name, timestamps, accumulated play time, game version, chapter label, and save-time thumbnail; autosave triggers for checkpoints, scene loads, a throttled timed interval, pause and quit, and manual calls.
- Load validation before every load: unreadable or newer-version saves shown unavailable with a plain-language reason.
- Debug console: attribute and programmatic (`Register`) command registration; built-in help, clear, echo, quit, timescale, fps and status commands; history and completion; readable answers instead of exceptions; audience gating; `IncludeInReleaseBuilds` strip for release builds (fresh-install default: development only).
- GlueKit Playground sample: the five-action run — lower the music, rebind Jump to F, checkpoint autosave, save "First run" to Slot 1, `gluekit.give key` and open the locked door.
- Documentation set: quick-start, settings guide, input-rebinding guide, save-slots guide, debug-console guide (including the numbered release-strip procedure), "what v1 is not", full reference.
- 47 automated EditMode tests (NUnit) green on Unity 6 — development project and clean project; player self-tests passing in development, release, and clean-project Windows builds.
- Unity 6 only (6000.0+). Dependencies: Unity's Input System, UGUI and UI Toolkit only.
