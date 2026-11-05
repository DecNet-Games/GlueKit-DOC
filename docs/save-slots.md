---
layout: default
title: Save Slots
nav_order: 10
description: "Five manual slots plus a dedicated autosave slot manual saves can never overwrite — each slot carrying its name, timestamps, play time, game version, chapter label and a thumbnail captured at save time."
---

# Save Slots
{: .no_toc }

GlueKit's save system is a **framework your game hangs its own data on**: GlueKit owns the slots, the metadata, the autosave triggers and the load validation; your game owns what a save means.

## The slots

- **Five manual slots**, saved and loaded deliberately by the player.
- **One dedicated autosave slot** that manual saves can **never overwrite** — the autosave is always there even if the player fills every manual slot.

## What every slot carries

- The slot's **name** (players can rename a slot in the panel — "First run" in the Playground is exactly this).
- **Timestamps** for the save.
- **Accumulated play time**.
- The **game version** that wrote the save — the value [load validation]({{ site.baseurl }}/docs/load-validation/) checks before a load.
- A **chapter label** your game sets, so a slot can say where in the game it belongs.
- A **thumbnail captured at save time**, so the slot panel shows the moment, not just numbers.

## The boundary, stated plainly

The save leg is **slots, autosave, and load validation**. It is not save migration, not cloud sync, not corruption recovery, and it does not encrypt saves — that depth is a different tool's job, and [What v1 Is Not]({{ site.baseurl }}/docs/what-v1-is-not/) says so in the package itself. The Home window's Save Slots section shows the save data root and every slot's state.
