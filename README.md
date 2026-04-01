# Design Engineering

This repo is the operating system for the next phase of your work.

It is not the product repo.
It is where you decide:

- what to build
- why it matters
- which stack to use
- how the work should be packaged
- how the public story should evolve

The current product focus is:

`toolmotion` — a motion system for complex tools

That means:

- `design-engineering` is strategy, specs, writing, and roadmap
- `toolmotion` is the implementation repo
- `toolmotion` lives in its own separate repository

## Core Thesis

The strongest public story is:

`I build AI-native tools with strong interaction design across iOS, web, and CLI.`

The current wedge into that story is:

`interaction systems for complex tools`

## How To Use This Repo

Use this repo as a living workspace for:

- product briefs
- architecture decisions
- stack choices
- roadmap checkpoints
- writing drafts
- portfolio cleanup
- new project proposals

Do not treat it like a dump of random ideas.
Every file should help answer a real decision.

## Main Files

- `PRESENT.md`
  Current state of the portfolio and GitHub profile.
- `VISION.MD`
  Long-term direction and what this work is trying to become.
- `TECHSTACK.MD`
  Stack decisions for `toolmotion` and adjacent projects.
- `ROADMAP.MD`
  Execution plan for the next 90 days.
- `PROFILE_README.md`
  Draft GitHub profile copy.
- `REPO_TRIAGE.md`
  What to keep public, archive, rename, or de-emphasize.

## Working Rules

- fewer repos
- clearer names
- fewer experiments made public
- more proof in the work that stays public
- more writing tied to shipped artifacts
- build systems, not isolated demos

## Current Decision

We are not building a generic component library first.

We are building:

1. a motion system
2. a pattern library for serious software
3. a demo app proving those patterns
4. framework adapters only after the semantics are stable

## Framework Decision

`toolmotion` should be super-focused.

That means:

- core package: framework-agnostic `TypeScript`
- first adapter: `React`
- first demo environment: `Vite`
- later product consumer: maybe `Redwood`

`Redwood` is not rejected.
It is just not the foundation of the system itself.

Use Redwood later for:

- a product app that consumes `toolmotion`
- a workflow console
- an AI/devtools application

Do not use Redwood to define the initial public motion system.

## Immediate Next Step

Open the separate `toolmotion` repository.

That is where the current product work lives.
