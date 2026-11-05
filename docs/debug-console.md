---
layout: default
title: The Debug Console
nav_order: 13
description: "An extensible in-game console: attribute or programmatic command registration, history and completion, readable answers instead of exceptions, and audience gating that decides who can open it."
---

# The Debug Console
{: .no_toc }

Testing without a console means rebuilding for every cheat. GlueKit's console is the in-game surface for that work — and it is built to be extended by your game, not just used as shipped. (In v1 the console ships in **UGUI form only**; the settings, controls, and slot menus ship in both UGUI and UI Toolkit.)

## Built for your commands

Register commands with an **attribute** on your method, or with a single programmatic **`Register`** call. See [Console Commands]({{ site.baseurl }}/docs/console-commands/) for the built-in set and the registration routes.

## Behaviour in the room

- **History** — previous commands are kept, so the test loop is type-less, arrow-more.
- **Completion** — command names complete as you type.
- **Readable answers, never exceptions** — an unknown command or a bad argument gets a readable line back, not a stack trace in your tester's face.

## Audience gating

**Audience gating decides who can open the console** — the console is a development tool, and who counts as its audience is your call. And when the game ships, one setting removes the console from the build entirely: see [Stripping the Console from Release Builds]({{ site.baseurl }}/docs/release-strip/). The Home window's Debug Console section shows the console's audience and release-strip state.
