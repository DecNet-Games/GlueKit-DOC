---
layout: default
title: One-Click Setup
nav_order: 6
description: "One action generates GlueKit's profiles and settings assets in your project — and running it again recognises the existing setup and preserves the values you edited."
---

# One-Click Setup
{: .no_toc }

Setup is the single action on GlueKit Home's Welcome block. It generates what the four systems need inside your project — the settings profiles, generated settings assets, and the sample-ready state — under one persistence root the whole package shares.

## Safe to run twice

Setup is **idempotent**. Run it a second time and it recognises the existing setup (`alreadySetUp`) instead of rebuilding over it: values you edited in your profiles are preserved, and an already-imported Playground is reported as already imported rather than duplicated. This behaviour is covered by an automated test (setup run twice in the development project and in a clean foreign project) — setup never punishes you for pressing the button again.

## What setup verifies

The Welcome block verifies the install after setup: the four legs initialise against the generated assets, and [Leg Status]({{ site.baseurl }}/docs/home-window/) shows each system's state. If a leg is not ready, the window says which one — you do not have to guess which system is unconfigured.
