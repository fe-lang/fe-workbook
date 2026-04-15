# Lesson 01 — Language Basics

Each file in this directory is a small, intentionally broken Fe program. Fix the `PROBLEM:` markers until `fe check` succeeds.

## Goal

Practice basic language features:

- contract messages and selectors (`msg`, `recv`)
- effects and capability scoping (`uses (...)`, `with (...)`)
- borrow handles (`mut` / `ref`) and overlap rules
- types: exhaustive `match` and trait bounds
- higher-kinded types (kinds like `* -> *`) with `Functor`/`Applicative`

## Exercises

- `00-messages.fe` — Fix missing/duplicate message selectors.
- `01-effects.fe` — Fix missing effect declarations and mutability issues.
- `02-types.fe` — Make a `match` exhaustive and add a trait bound.
- `03-hkts.fe` — Add a kind bound and type annotations for `Result`.
- `04-borrows.fe` — Fix borrow conflicts by copying from `ref` handles and managing reborrows.

## Run

From the repo root:

```bash
cd lessons/01-language
fe check 00-messages.fe
fe check 01-effects.fe
fe check 02-types.fe
fe check 03-hkts.fe
fe check 04-borrows.fe
```
