---
layout: default
title: Troubleshooting
nav_order: 19
description: "The states GlueKit reports about itself: a leg that is not ready in Leg Status, an unavailable save and its reason, an unbound required action, and a console that is absent from a release build on purpose."
---

# Troubleshooting
{: .no_toc }

## A system shows as not ready in GlueKit Home

[Leg Status]({{ site.baseurl }}/docs/home-window/) names the leg that is not ready. The usual cause is that [setup]({{ site.baseurl }}/docs/one-click-setup/) has not run yet in this project — run it once; setup is idempotent, so running it again never overwrites the profile values you edited.

## A save slot shows as unavailable

That is [load validation]({{ site.baseurl }}/docs/load-validation/) working. The slot failed its pre-load check — it cannot be read, or a newer game version wrote it — and the panel shows the reason in plain language next to the slot. The save is not loaded over the player's progress, and the other slots are unaffected.

## A required action is unbound

The rebind panel **flags** a required action left unbound instead of letting it slide — capture a binding for it in [Key Rebinding]({{ site.baseurl }}/docs/key-rebinding/), or use Reset All Bindings to return to the shipped defaults. (Reset All Bindings is separate from Restore Defaults, which never touches bindings.)

## The console does not open in my release build

That is the intended state if `IncludeInReleaseBuilds` is off: the console is stripped from release builds and has no open path there. Check the audience and strip state in the Home window's Debug Console section, and see [Stripping the Console from Release Builds]({{ site.baseurl }}/docs/release-strip/).

## My settings menu and my controls show different values

They cannot drift: both menu stacks (UGUI and UI Toolkit) render the **same settings model**. If a value looks wrong, check which settings profile is active in the Home window's Settings section — the menus show the active profile's values.
