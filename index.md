---
layout: home
title: Home
nav_order: 1
description: "GlueKit is settings, controls, save slots and a debug console for Unity 6 — the four systems every game needs before it ships, in one package with one setup and one sample."
permalink: /
---

# GlueKit
{: .fs-9 }

**Settings, controls, save slots and a debug console** — the systems every game needs before it ships, in one maintained package for Unity 6.
{: .fs-6 .fw-300 }

[Get started]({{ site.baseurl }}/docs/getting-started/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }
[Buy on the Unity Asset Store](https://assetstore.unity.com/publishers/118262){: .btn .fs-5 .mb-4 .mb-md-0 }

---

## The week every prototype reaches

Every playable prototype reaches the same week. The game is fun in the room, and then it needs a settings menu players can open without embarrassment, key rebinding because players are already asking for it, save slots because a single autosave is no longer enough, and a debug console because testing without one means rebuilding for every cheat. Each of those is sold separately, at fragment prices, with its own setup and its own idea of how your game should be organised. GlueKit is the four of them as one system: one setup action, one persistence root, one sample, one publisher maintaining them together across Unity 6 updates.

- **A complete settings system** — graphics, audio, gameplay and accessibility settings defined once, as data, and generated as working menus in both UGUI and UI Toolkit, on the same live model. Graphics presets drive your URP or HDRP Volume profile as well as the quality level, and take effect at runtime without a scene reload.
- **Rebinding on the Input System your project already uses** — per-scheme bindings, keyboard and gamepad glyphs with text fallback, and real conflict handling: capture a key another action already uses and the panel names the conflict and offers **Swap**, **Replace**, or **Cancel**. A binding is never silently stolen.
- **Save slots and autosave, as a framework** — five manual slots plus a dedicated autosave slot that manual saves can never overwrite. Slot name, timestamps, accumulated play time, game version, chapter label and a thumbnail captured at save time. Before a save can be loaded it is validated, and a save that cannot be loaded is shown as unavailable with the reason in plain language.
- **A debug console your game can extend** — register commands with an attribute or a single `Register` call. History, command completion, audience gating — and one setting, `IncludeInReleaseBuilds`, that strips the console from release builds. The default for a fresh install is development only.

## See it work in one session

The **GlueKit Playground** ships in the package: a small walkable yard with a checkpoint arch, a locked door, and a prompt card listing five things to try. Lower the Music Volume and hear it drop; rebind Jump from Space to F and jump with F; walk through the checkpoint and watch the autosave slot appear; save manually into Slot 1 and rename it "First run"; open the console, type `gluekit.give key`, and open the locked door. That run is the demo, the onboarding, and the proof that all four systems work together. See [The Playground Sample]({{ site.baseurl }}/docs/playground/).

## One window for all of it

**Tools → Decnet Games → GlueKit** opens GlueKit Home: a welcome block with one-click setup and verification, a **Leg Status** section that answers "what state is my glue in?" at a glance, and a section per system. See [The Home Window]({{ site.baseurl }}/docs/home-window/).

> Automated verification for v1.0.0: **47/47** EditMode tests green on Unity 6, in the development project and in a clean project. The Playground's five-action run passes end-to-end in built Windows players — development build (10/10 self-test steps) and release build, with the console stripped. GlueKit v1 is a **Unity 6 only** package — it does not support Unity 2022.3 or earlier. See [What v1 Is Not]({{ site.baseurl }}/docs/what-v1-is-not/).
