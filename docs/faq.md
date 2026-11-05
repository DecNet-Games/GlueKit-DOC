---
layout: default
title: FAQ
nav_order: 18
description: "Short answers: Unity versions, the Input System requirement, what the save system does and does not do, the release strip, menu stacks, and what verification actually ran."
---

# FAQ
{: .no_toc }

## Does GlueKit work on Unity 2022.3?

No. GlueKit v1 is a **Unity 6 only** package (6000.0 and later). See [What v1 Is Not]({{ site.baseurl }}/docs/what-v1-is-not/).

## My project uses the legacy Input Manager. Can I use the rebinding?

No — rebinding is built on Unity's **Input System** package. Legacy Input Manager projects are not supported in v1.

## Is this a full save-game system — migration, cloud saves, encryption?

No. The save leg is **slots, autosave, and load validation**: five manual slots, a protected autosave slot, rich slot metadata, and a validation check before any load. It does not migrate saves between versions, sync to a cloud, recover corrupted saves, or encrypt anything. Your game hangs its own save data on the framework.

## How does the console get out of my release build?

One setting: `IncludeInReleaseBuilds`. With it off (the fresh-install default), the console removes itself at startup in a non-development player — no surface, no open path. The full procedure is in [Stripping the Console from Release Builds]({{ site.baseurl }}/docs/release-strip/).

## Which UI stack do the menus use?

Both. Settings, controls, and slot menus are generated for **UGUI and UI Toolkit** from the same data and the same live model. The one exception is the debug console, which ships in UGUI form only in v1.

## What platforms are verified?

The **Unity 6 Editor** and **Windows PC player builds** — development, release (console stripped), and a clean project's player, with the Playground's five-action run passing end-to-end in each. GlueKit makes no console, mobile, or WebGL claim.

## What dependencies does GlueKit add?

Unity's own packages only: **Input System, UGUI, and UI Toolkit**. No third-party dependencies.
