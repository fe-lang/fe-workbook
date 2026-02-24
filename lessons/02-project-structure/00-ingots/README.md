# Exercise 00 — Ingots (packages)

This exercise uses two ingots:

- `utils/` — a tiny library ingot
- `app/` — depends on `utils/` (via an alias) and has a nested module

## Goal

Learn:

- the standard ingot layout: `fe.toml` + `src/lib.fe`
- dependency **alias** vs ingot **name** (imports start from the alias)
- modules: a module root is a `*.fe` file (e.g. `src/messages.fe`)
- submodules: a module can have a same-named directory for its children (e.g. `src/messages/transfer.fe`)

## Run

From the repo root:

```bash
cd lessons/02-project-structure/00-ingots
fe check app
```

## Fix

1. Fix the import in `app/src/lib.fe` to use the dependency alias from `app/fe.toml`.
2. Make the `messages` module resolvable.

## Hints

- Start by reading `app/fe.toml` to see the alias for the `utils` ingot.
- For module discovery, the directory `src/messages/` is not enough on its own: Fe also needs a `src/messages.fe` module root.
- `fe tree app` can be handy for visualizing what the compiler thinks the module layout is.

## Done

```bash
fe check app
```
