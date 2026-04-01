# GitHub Profile Plan

As of April 1, 2026.

This document answers three questions:

1. What should the public profile say?
2. Which repos should stay public, get archived, or go private?
3. What should you build or polish next?

## The Public Story

Use this as the center of gravity:

`I build AI-native tools with strong interaction design across iOS, web, and CLI.`

Expanded version:

`Design engineer and product-minded systems builder working across iOS, web, and terminal. I make complex workflows fast, legible, and trustworthy.`

That is the story.
Do not lead with “I know many languages.”
Do not lead with “I am exploring everything.”

## Recommended GitHub Profile README

Use something close to this:

```md
# senik

I build AI-native tools with strong interaction design across iOS, web, and CLI.

I care about:
- interaction systems for complex tools
- native Apple software
- developer experience and terminal products
- AI interfaces with strong trust, visibility, and feedback

## Selected Work

- [recap](https://github.com/stussysenik/recap) — capture terminal sessions and export them as polished PDFs and PNGs
- [vfx](https://github.com/stussysenik/vfx) — terminal-native graphics engine with high-quality real-time effects
- [dcal](https://github.com/stussysenik/dcal) — macOS display calibration utility with color and analysis tooling
- [MusicBrowser](https://github.com/stussysenik/MusicBrowser) — refined iOS/macOS music browser built with SwiftUI and MusicKit

## Current Focus

- building tools for human + AI workflows
- designing motion and interaction systems for utility software
- shipping native and terminal software that feels unusually good to use

## Writing

Notes on internal tools, interaction systems, motion, and AI-native UX:
- coming soon
```

## Pinned Repos

Pin exactly `4`.

Recommended:

- `recap`
- `vfx`
- `dcal`
- `MusicBrowser`

If you want a more research-heavy version, swap one of the above for:

- `bboy-analytics`
- `e-nable`
- `chrono-type`

Do not pin:

- forks
- generic playgrounds
- clones
- repo names that read like prompts

## Repo Triage

### Keep Public And Polish First

These are the strongest public assets:

- `recap`
- `vfx`
- `dcal`
- `MusicBrowser`
- `e-nable`
- `chrono-type`
- `bboy-analytics`
- `lua-breaking`
- `portfolio-forever`

These should each have:

- clean README
- sharp title and one-line description
- screenshots or demo GIF
- install/run instructions
- architecture notes only if useful
- license
- issues cleaned up

### Keep Public But Lower Priority

- `dumpling-not-dumpling`
- `breakdex`
- `mit-ocw-reels`
- `zigshot`
- `ghost-tracks`

These are fine to keep public if you like them, but they should not define your profile.

### Make Private Or Archive

These weaken the public story unless they are elevated significantly:

- `windmill-portfolio`
- `webgpu-sprites-animation-library-vue-cli-everything-everywhere-cli-web`
- small `*-playground` repos that are not supporting an active flagship
- clone-heavy variants like `mymind-clone-web`
- duplicate rewrites like `redwood-*` experiments that do not add a distinct thesis
- generic coursework-era projects that do not help the current story

Likely archive/private candidates:

- `Weather-jounal-app-UDACITY`
- `WhackAMole`
- `Chuck-Norris`
- `Capstone`
- `fend-boilerplate`
- `flipmakers`
- `attendu-showreel`
- `windmill-portfolio`
- `webgpu-sprites-animation-library-vue-cli-everything-everywhere-cli-web`
- `typescript-playground`
- `lua-playground`
- `lisp-playground`
- `perplexica-playground`
- most tiny `playground`, `clone`, and `study` repos with no serious packaging

### Rename Or Reframe

- `portfolio-forever` -> `stussysenik.com`
- `windmill-portfolio` -> `windmill-ui-study` if kept public
- `breakdex` -> `breakdex-ios`
- `webgpu-sprites-animation-library-vue-cli-everything-everywhere-cli-web` -> `sprite-atelier` if kept at all
- `vfx` can stay if you intend to keep the brand; otherwise `termfx`

## What To Polish Right Now

### 1. `recap`

This is one of the best signals on the profile.

Why:

- useful
- devtool-shaped
- clear problem
- differentiated
- easy to explain

Polish tasks:

- tighten the README headline and install story
- add a “why this exists” section
- improve demo assets
- package release/install paths clearly
- show real examples from actual engineering workflows

### 2. `vfx`

This is your most distinctive craft artifact.

Why:

- motion
- graphics
- terminal
- constraints-driven engineering
- aesthetic judgment

Polish tasks:

- make the effect gallery exceptionally clean
- add performance notes and architecture explanation
- position it as a terminal interaction/graphics primitive, not just a demo reel
- consider whether it can feed another project as infrastructure

### 3. `dcal`

This is strong because it reads like real software for serious users.

Why:

- macOS utility
- color/science angle
- design-aware toolmaking
- not generic

Polish tasks:

- tighten onboarding
- make screenshots more product-like
- make use cases explicit
- show the interaction model, not just features

### 4. `MusicBrowser`

This is your best current iOS/macOS product signal.

Polish tasks:

- make the README feel complete and senior
- add architecture and tradeoff notes
- show careful platform decisions
- emphasize why it exists beyond being “Marvis-inspired”

## What To Build Next

### Highest-Value Project

Build:

`Operator`

A polished workflow and artifact console for teams working with AI and engineering automation.

This should be:

- keyboard-first
- dense but legible
- CLI + web connected
- designed around runs, logs, plans, diffs, outputs, approvals, and previews
- suitable for Windmill-like workflows

Why this project:

- it directly matches your strongest skill
- it is relevant to Windmill
- it bridges design engineering, devtools, AI interfaces, and systems
- it proves product thinking better than another visual study

### Second Project

Build:

`Motion System for Tools`

A set of reusable interaction patterns for:

- interruption
- spring behavior
- state continuity
- reduced motion
- background tasks
- progress and completion

Targets:

- SwiftUI
- React
- terminal patterns if useful

Why:

This converts your taste into reusable primitives.
That is staff-level signal.

### Third Project

Build:

`AI-native iOS Utility`

Not chat.
Not a novelty classifier.

A real app that takes camera, screenshot, or text input and turns it into structured action.

Examples:

- screenshot to task/issue organizer
- receipt/doc/image to reviewed structured data
- camera-based workflow helper with local or hybrid inference

Why:

This strengthens the Apple-native lane and the applied AI lane at the same time.

## What To Stop Working On

Stop spending serious time on:

- one-off clones
- tiny playground repos
- framework rewrites of the same idea
- language collecting as public identity
- pure visual trend work with no product consequence

## Packaging Rules

Every repo you keep public should answer these in the first screenful:

- what is it
- who is it for
- why does it exist
- how do I run it
- what makes it different

Every serious repo should also have:

- license
- screenshots/demo
- install instructions
- “status” note
- roadmap only if credible and short

## The Short Recommendation

If you do only five things:

1. Rewrite the GitHub profile README.
2. Re-pin the top four repos.
3. Archive or private the obvious low-signal repos.
4. Polish `recap`, `vfx`, `dcal`, and `MusicBrowser`.
5. Build `Operator` as the flagship that ties your whole story together.

