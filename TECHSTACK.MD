# TECHSTACK

As of April 1, 2026.

This document answers one question:

`What stack should we use for toolmotion and why?`

## Short Answer

Use:

- `TypeScript` for the core package
- `React` for the first adapter
- `Vite` for the demo app
- `motion` for concrete React examples
- `Vitest` for package tests
- `Playwright` later for visual checks

Do not start with:

- Go
- Elixir
- Zig
- Lua
- Redwood
- SvelteKit
- Remix

Those may be useful later, but they are not the right `v1` stack for community adoption.

## Decision Summary

The stack decision is:

- `TypeScript` is the core
- `React` is the first public adapter
- `Vite` is the first demo environment
- `Redwood` is downstream, not foundational

`toolmotion` should stay super-focused.

It should not become:

- a framework thesis
- a full-stack app
- a Redwood showcase
- a multi-runtime experiment

It should become:

- a reusable motion system
- a pattern library for serious software
- an easy thing for frontend engineers to try

## The Product Shape

`toolmotion` is not a component library first.

It is:

1. a motion system
2. a pattern library
3. a docs and demo surface
4. a set of adapters

The order matters.

If you jump to components too early, you freeze abstractions before the motion semantics are proven.

## Recommended Stack By Layer

### 1. Core System

Use:

- `TypeScript`

Why:

- easiest community adoption
- best fit for frontend design engineers
- easy to publish as npm package
- easy to keep framework-agnostic

This layer should export:

- semantic tokens
- spring presets
- named patterns
- utility helpers

### 2. First Adapter

Use:

- `React`
- `motion`

Why:

- largest practical adoption surface
- strongest fit for design engineering teams
- easiest way to prove patterns in live interfaces

This layer should be:

- optional
- thin
- clearly separate from the core package

### 3. Demo App

Use:

- `Vite`
- `React`
- `TypeScript`

Why:

- fastest loop
- minimal ceremony
- best fit for pattern exploration
- no need for SSR complexity yet

The demo app should prove:

- command menu
- inspector panel
- toast stack
- row insert/remove
- modal choreography
- progress and completion swaps

### 4. Docs

Use one of two approaches:

- start simple with repo docs and demo app
- later add a docs site if the project gains traction

Do not overbuild docs infrastructure before the patterns are good.

## What About SvelteKit?

SvelteKit is a good choice for a content-forward site.
It is not my first choice for `toolmotion v1`.

Why:

- the first adapter should target React
- the demos should live in the same ecosystem as the main adopter story
- too many frameworks too early weakens focus

Use SvelteKit later only if you want:

- a polished public docs site
- writing + demos together
- a more editorial project site

## What About Redwood?

Redwood is better for product applications than for a motion-system library.

If the question is:

`Should Redwood be the core of toolmotion?`

The answer is:

`No.`

Use Redwood when you build a full product like:

- `Operator`
- an AI workflow console
- a real internal-tool or product app

Do not use it for `toolmotion v1`.

Why:

- `toolmotion` needs the smallest possible public surface area
- the core should be easy to publish and easy to adopt
- React users should be able to try it without entering a larger framework story
- framework coupling too early weakens the community value

So the correct shape is:

- core system first
- React adapter second
- real product app later

That later product app can absolutely be built in Redwood if it is the right product choice.

## What About Remix?

Remix is strong for product apps and web fundamentals.
It is still not the right first move here.

Same reason:

- library first
- adapter second
- demo app third

Use Remix later only if a real product demands it.

## What About Go?

Go is not needed for `toolmotion v1`.

Use Go only if you later want:

- a CLI
- code generation
- screenshot/video automation
- benchmark tooling
- release tooling

Go is a great support language.
It is not the core language for this project.

## What About Zig?

Zig is interesting for:

- tiny WASM helpers
- performance-sensitive kernels
- image or timing experiments

But again:

not for `v1`

If you use Zig too early, the project becomes more about the stack than the value.

## What About Lua?

Lua is worth respecting.
The philosophy is real:

- tiny footprint
- excellent embeddability
- expressive power per byte
- great fit for simulation, games, scripting, and tools

So why not go all in on Lua here?

Because `toolmotion` is trying to become a broadly usable community artifact for design engineers and frontend teams.

For that, the best adoption path is:

- npm package
- React examples
- TypeScript types
- easy copy-paste patterns

Lua is still valuable, but in a different role:

- research playgrounds
- motion simulations
- Love2D explorations
- interaction experiments
- future runtime experiments

So the rule is:

- `TypeScript` for the public system
- `Lua` for private labs or side research

## Community Use Format

Community adoption should happen in layers:

### Layer 1

Import tokens and patterns directly:

- `durations`
- `springs`
- `getPattern("panel")`

### Layer 2

Use React helpers:

- `toolmotion/react`

### Layer 3

Copy recipe patterns from docs:

- command menu recipe
- inspector recipe
- toast recipe
- validation recipe

### Layer 4

Eventually use platform companions:

- SwiftUI notes
- terminal patterns
- framework examples

## Final Decision

For now:

- `TypeScript` is the core
- `React + motion` is the first adapter
- `Vite` is the demo environment
- `Redwood` is reserved for downstream product apps
- `Lua`, `Go`, `Zig`, `Elixir`, `SvelteKit`, and `Remix` stay out of the critical path

That is how we keep the project focused and legible.
