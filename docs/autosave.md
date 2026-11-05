---
layout: default
title: Autosave
nav_order: 11
description: "Autosave triggers for the moments games actually need: checkpoints, scene loads, a throttled timed interval, pause and quit, and manual calls — always into the dedicated autosave slot."
---

# Autosave
{: .no_toc }

Autosaves always land in the **dedicated autosave slot** — the one manual saves can never overwrite (see [Save Slots]({{ site.baseurl }}/docs/save-slots/)). Your game decides which triggers it uses:

- **Checkpoints** — the trigger the Playground demonstrates: walk through the checkpoint arch and the autosave slot appears with its timestamp and thumbnail.
- **Scene loads** — a save as the game moves between scenes.
- **A throttled timed interval** — periodic autosaves, throttled so the timer cannot hammer the disk.
- **Pause and quit** — a save when the player pauses, and a last save on the way out.
- **Manual calls** — your code asks for an autosave at the moment that makes sense for your game.

Every autosave is a normal GlueKit save: it carries the slot metadata (timestamps, play time, game version, chapter label, thumbnail) and passes through the same [load validation]({{ site.baseurl }}/docs/load-validation/) before it can ever be loaded back.
