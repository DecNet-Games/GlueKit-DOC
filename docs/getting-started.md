---
layout: default
title: Getting Started
nav_order: 2
description: "From the Asset Store download to all four systems working together: install GlueKit, run the one-click setup, and play the Playground's five-action run."
---

# Getting Started
{: .no_toc }

GlueKit works in one Editor window and one loop: **set up** once, then use the four systems — **settings**, **rebinding**, **save slots**, **debug console** — from the same home window and the same persistence root. This section takes you from the Asset Store download to all four systems working together in the shipped sample.

## The path

1. [Install]({{ site.baseurl }}/docs/installation/) the package from the Unity Asset Store.
2. Follow the [Quick Start]({{ site.baseurl }}/docs/quick-start/): open GlueKit Home, run the one-click setup, and play the Playground.
3. Learn the one window in [The Home Window]({{ site.baseurl }}/docs/home-window/).

## What GlueKit needs from you

- A Unity **6** project (6000.0 or later). GlueKit v1 is a Unity 6 package and does not support Unity 2022.3 or earlier — stated plainly, because it decides whether the package is for you at all.
- Unity's own packages only: **Input System**, **UGUI**, and **UI Toolkit**. There are no third-party dependencies. Projects on the legacy Input Manager are not supported in v1.

## The honest frame, up front

The four systems are runtime systems — they work in your built game, not only in the Editor. GlueKit's save system is slots, autosave, and load validation: it is not a save-migration, cloud-sync, or corruption-recovery system, and it does not encrypt saves. The debug console ships in UGUI form only in v1. GlueKit ships English only and is verified for Windows PC players. The full boundary list is in [What v1 Is Not]({{ site.baseurl }}/docs/what-v1-is-not/) — and the same page ships inside the package itself.
