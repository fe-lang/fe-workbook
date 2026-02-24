# Exercise 01 — Workspaces

This exercise is a small workspace with two members (`math/` and `app/`) plus a vendored dependency under `vendor/`.

## Goal

Understand workspace mechanics:

- a workspace root `fe.toml` selects multiple ingots ("members")
- members can be constrained by expected `name`/`version` (mismatches are errors)
- workspace-level dependency aliases must not conflict with member names

## Run

From the repo root:

```bash
cd lessons/02-project-structure/01-workspaces
fe check .
```

## Fix

1. Fix the workspace member metadata mismatch (the workspace expects `math@0.1.0`).
2. Fix the workspace dependency alias conflict (workspace deps can't reuse member names).

## Hints

- Both issues are in the workspace root `fe.toml`.
- After fixing the workspace, `app/` should be able to resolve `math = true` as a workspace member dependency.

## Done

```bash
fe check .
```

## Extra (CLI targeting)

From inside the workspace root you can also target a member by **name**:

```bash
fe check math
fe check app
```
