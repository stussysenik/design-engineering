# ROADMAP

As of April 1, 2026.

This roadmap is for the next 90 days.

The main objective is:

`make toolmotion real enough that other people can understand, try, and eventually adopt it`

## Repo Roles

### design-engineering

Use this repo for:

- vision
- stack decisions
- roadmap
- writing drafts
- repo triage
- public-positioning decisions
- future product proposals

### toolmotion

Use this repo for:

- implementation
- demos
- package code
- adapters
- examples

## Phase 1: Clarify And Focus

Goal: make the direction unambiguous.

Tasks:

- finalize `VISION.MD`
- finalize `TECHSTACK.MD`
- finalize `ROADMAP.MD`
- align the GitHub profile story with the motion-system direction
- stop spawning unrelated public experiments

Definition of done:

- the repo explains what we are doing
- the stack is chosen
- the next 3 milestones are obvious

## Phase 2: Build The Demo App

Goal: prove the system in realistic software surfaces.

Build these first:

1. command menu
2. inspector panel
3. toast stack
4. row insert/remove
5. progress state handoff

Rules:

- every demo must feel like serious software
- every demo must support reduced motion
- every demo must be keyboard-aware where relevant
- do not add decorative motion

Definition of done:

- demos are interactive
- patterns feel coherent
- before/after value is obvious

## Phase 3: Turn The Demos Into A Usable System

Goal: make the package feel real.

Tasks:

- refine tokens
- refine spring presets
- improve naming
- add docs for when not to animate
- add React adapter helpers if the demos justify them

Definition of done:

- patterns are easy to explain
- the exports are stable enough for others to try
- there is a clear “how to use this” story

## Phase 4: Public Proof

Goal: make `toolmotion` legible to the community and to hiring managers.

Tasks:

- write one essay tied to the project
- publish a demo video
- add screenshots and pattern explanations
- integrate the system into one real surface

Definition of done:

- someone can understand the value without reading all the code
- the project looks intentional
- the project shows taste and technical reasoning

## Phase 5: Profile Cleanup

Goal: make the public account match the new center of gravity.

Tasks:

- update GitHub profile README
- set pins correctly
- archive or de-emphasize low-signal repos
- polish the strongest repos

Definition of done:

- the profile reads as focused
- the account no longer feels scattered

## The One Rule

Do not start a new flagship until `toolmotion` has:

- a real demo app
- a coherent package shape
- a clear README
- one strong essay

## What Comes After

Once `toolmotion` is credible, choose one of:

- build `Operator`
- build a SwiftUI companion
- build a CLI or devtools companion
- integrate `toolmotion` into a real product app

Do not decide that early.
Earn the next move by finishing the current one.

