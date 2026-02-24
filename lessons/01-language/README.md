# Lesson 01 — Language Basics

Each file in this directory is a small, intentionally broken Fe program. Fix the `PROBLEM:` markers until the file compiles (and the tests pass, where present).

## Goal

Practice basic language features:

- contract messages and selectors (`msg`, `recv`)
- effects and capability scoping (`uses (...)`, `with (...)`)
- types: exhaustive `match` and trait bounds
- higher-kinded types (kinds like `* -> *`) with `Functor`/`Applicative`

## Exercises

- `00-messages.fe` — Fix missing/duplicate message selectors.
- `01-effects.fe` — Fix missing effect declarations and mutability issues.
- `02-types.fe` — Make a `match` exhaustive and add a trait bound.
- `03-hkts.fe` — Add a kind bound and type annotations for `Result`.

## Run

From the repo root:

```bash
cd lessons/01-language
fe test 00-messages.fe
fe test 01-effects.fe
fe test 02-types.fe
fe test 03-hkts.fe
```
