---
layout: default
title: Stripping the Console from Release Builds
nav_order: 15
description: "One setting — IncludeInReleaseBuilds — strips GlueKit's console from release builds. The fresh-install default is development only, and the strip is verified in a real release player."
---

# Stripping the Console from Release Builds
{: .no_toc }

A debug console is a development tool. Shipping it — even hidden behind a key combination — ships a surface your players were never meant to reach. GlueKit removes it by setting, not by discipline.

## The setting

**`IncludeInReleaseBuilds`** controls whether the console exists in release builds. The default for a fresh install is **development only, stripped from release**.

## How the strip works

In a non-development player with `IncludeInReleaseBuilds` off, the console removes itself at startup — before it creates any controller or visuals, it deletes its own surface and deactivates, so **no console surface and no open path exists in the running release game**. There is nothing to "find" with the right keypress, because there is nothing there.

The package's debug-console guide carries the **numbered strip procedure and how to verify the strip** in your own build. The mechanism is also how GlueKit's own verification ran: the release-build player self-test passes with the check "console-stripped: overlay absent" while every other system still initialises and works.

## The honest scope of the strip

Stripping removes **GlueKit's console surface** from your release build. Your own command code remains your game's code — what your commands do, and whether the code behind them ships, is your game's own decision.
