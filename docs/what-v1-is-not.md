---
layout: default
title: What v1 Is Not
nav_order: 17
description: "GlueKit v1's explicit boundaries: Unity 6 only, a save leg that is slots/autosave/validation and nothing deeper, a UGUI-only console, and the platforms that are not claimed."
---

# What v1 Is Not
{: .no_toc }

This page ships inside the package as well as here. GlueKit v1's boundaries, stated before you buy rather than after:

- **Not a Unity 2022.3 package.** GlueKit v1 is Unity 6 only (6000.0 and later). It does not support Unity 2022.3 or earlier, and no part of the copy pretends otherwise.
- **Not a deep save system.** The save leg is slots, autosave, and load validation. It is **not** save migration, **not** cloud sync, **not** corruption recovery, and it does **not** encrypt saves or claim tamper protection. If your game needs that depth, it is a different tool's job.
- **Not verified beyond Windows PC players.** Verification ran on the Unity 6 Editor and in Windows PC player builds. GlueKit makes **no console, mobile, or WebGL claim**.
- **Not a both-stacks console.** The debug console ships in UGUI form only in v1. The settings, controls, and slot menus ship in both UGUI and UI Toolkit — the console does not, yet.
- **Not legacy-input compatible.** Rebinding is built on Unity's Input System; projects on the legacy Input Manager are not supported in v1.
- **Not localised.** GlueKit ships English only.
- **Not a third-party integrator.** GlueKit does not claim compatibility with other save or input products; its dependencies are Unity's own packages only — Input System, UGUI, and UI Toolkit.
