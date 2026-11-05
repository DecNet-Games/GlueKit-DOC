---
layout: default
title: Console Commands
nav_order: 14
description: "The shipped command set — help, clear, echo, quit, timescale, fps, and status, which prints each system's health in plain language — and the two routes for registering your own."
---

# Console Commands
{: .no_toc }

## The shipped set

| Command | What it does |
|---|---|
| `help` | Lists the registered commands. |
| `clear` | Clears the console output. |
| `echo` | Prints its argument back — the first test that the console is alive. |
| `quit` | Quits the game. |
| `timescale` | Reads and sets the game's time scale. |
| `fps` | Reports the current frame rate. |
| `status` | Prints **each system's health in plain language** — settings, bindings, saves and console reporting their own state, so one command answers "is my glue healthy?" inside the running game. |

The Playground's fifth action uses a game-side command, not a built-in: `gluekit.give key` is registered by the sample to hand the player the door key. See [The Playground Sample]({{ site.baseurl }}/docs/playground/).

## Registering your own

Two routes, both first-class:

- **Attribute registration** — mark a method with GlueKit's command attribute and it joins the registry.
- **Programmatic registration** — a single `Register` call from your code.

Unknown commands and bad arguments are answered with readable lines, never exceptions — a mistyped cheat should cost a tester a second, not a session. How the console behaves (history, completion, gating) is covered in [The Debug Console]({{ site.baseurl }}/docs/debug-console/); how to remove the console from a shipped build is in [Stripping the Console from Release Builds]({{ site.baseurl }}/docs/release-strip/).
