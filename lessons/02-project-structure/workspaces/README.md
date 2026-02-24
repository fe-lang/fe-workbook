# 06 — Workspaces

## Goal

Understand workspace mechanics:
- a workspace root `fe.toml` selects multiple ingots (“members”)
- members can be constrained by expected `name`/`version` (mismatches are errors)
- workspace-level dependency aliases must not conflict with member names

## Run

```bash
cd lessons/02-project-structure/workspaces
fe check .
```

## Fixes to make

1) Fix the workspace member metadata mismatch (the workspace expects `math@0.1.0`).
2) Fix the workspace dependency alias conflict (workspace deps can’t reuse member names).

When done:

```bash
fe check .
```

## Extra (CLI targeting)

From inside the workspace root you can also target a member by **name**:

```bash
fe check math
fe check app
```
