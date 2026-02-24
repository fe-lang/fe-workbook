# 05 — Ingots (packages)

This problem uses **two ingots**:
- `utils/` — a tiny library ingot
- `app/` — an ingot that depends on `utils/` and has a submodule

## Goal

Learn:
- ingot layout: `fe.toml` + `src/lib.fe`
- dependency **alias** vs ingot **name** (import root comes from the alias)
- modules: a module root is a `*.fe` file (e.g. `src/messages.fe`)
- submodules: a module can have a same-named directory for its children (e.g. `src/messages/transfer.fe`)

## Run

```bash
cd lessons/02-project-structure/ingots
fe check app
```

## Fixes to make

1) Fix the import to use the dependency alias from `fe.toml`.
2) Make the `messages` module resolvable (hint: add `src/messages.fe`).

When done:

```bash
fe check app
```
