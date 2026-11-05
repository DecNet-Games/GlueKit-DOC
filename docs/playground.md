---
layout: default
title: The Playground Sample
nav_order: 16
description: "The shipped sample: a walkable yard with a checkpoint arch, a locked door, and a prompt card of five things to try — the demo, the onboarding, and the proof in one scene."
---

# The Playground Sample
{: .no_toc }

The GlueKit Playground ships in the package, importable from the Samples section of [GlueKit Home]({{ site.baseurl }}/docs/home-window/): a small walkable yard with a **checkpoint arch**, a **locked door**, and a **prompt card** listing five things to try.

## The five actions

1. **Lower the Music Volume** in the settings menu — and hear it drop. ([The Settings System]({{ site.baseurl }}/docs/settings-system/))
2. **Rebind Jump from Space to F** in Controls, and jump with F. ([Key Rebinding]({{ site.baseurl }}/docs/key-rebinding/))
3. **Walk through the checkpoint** — the autosave slot appears with its timestamp and thumbnail. ([Autosave]({{ site.baseurl }}/docs/autosave/))
4. **Save manually into Slot 1 and rename it "First run".** ([Save Slots]({{ site.baseurl }}/docs/save-slots/))
5. **Open the console, type `gluekit.give key`, and open the locked door.** ([Console Commands]({{ site.baseurl }}/docs/console-commands/))

Do them in one session and you have exercised all four systems **together** — which is the point. Fragments can each demo well alone; the Playground is the proof that these four work as one package, on one persistence root, in a built game.

## How the sample is verified

The five-action run is the package's own player self-test journey: it passes end-to-end in the built development player (10/10 self-test steps), in the release player with the console stripped, and in a player built from a clean project after a fresh setup.
