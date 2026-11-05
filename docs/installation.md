---
layout: default
title: Installation
nav_order: 3
description: "Install GlueKit from the Unity Asset Store and run the one-click setup. GlueKit is sold exclusively through the Unity Asset Store."
---

# Installation
{: .no_toc }

## Asset Store only
{: .no_toc .text-delta }

GlueKit is sold and delivered **exclusively through the Unity Asset Store** (publisher: Decnet Games). There is no other download channel — if a copy of GlueKit came from anywhere else, it did not come from us.

## Install

1. Purchase GlueKit on the Unity Asset Store.
2. In Unity, open **Window → Package Manager**, select **My Assets**, download and import GlueKit into your project.
3. Open the window from **Tools → Decnet Games → GlueKit**. Everything GlueKit does lives in that one home window — see [The Home Window]({{ site.baseurl }}/docs/home-window/).
4. Run the [one-click setup]({{ site.baseurl }}/docs/one-click-setup/) once. Setup generates GlueKit's profiles and settings assets inside your project, and running it again recognises the existing setup instead of overwriting your edits.

## Requirements

- Unity **6** (6000.0 or later). GlueKit v1 does not support Unity 2022.3 or earlier.
- Unity packages: **Input System**, **UGUI**, and **UI Toolkit** — no third-party dependencies.
- Projects on the legacy Input Manager are not supported in v1; rebinding is built on the Input System.

## Verified state

Automated verification for v1.0.0 ran on Unity 6: **47/47** EditMode tests green in the development project and in a clean project, and the Playground's five-action run passes end-to-end in built Windows players (development 10/10 self-test steps; release build with the console stripped). GlueKit is verified on the Unity 6 Editor and in Windows PC player builds — it makes no console, mobile, or WebGL claim. See [What v1 Is Not]({{ site.baseurl }}/docs/what-v1-is-not/).
