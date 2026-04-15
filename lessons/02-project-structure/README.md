# Lesson 02 — Project Structure

Two exercises focused on how Fe projects are laid out on disk.

## Goal

- Understand ingot layout (`fe.toml`, `src/lib.fe`) and module discovery rules
- Understand workspaces: members, metadata constraints, and dependency alias rules

## Exercises

- Exercise 00 — Ingots (packages): `lessons/02-project-structure/00-ingots/README.md`
- Exercise 01 — Workspaces: `lessons/02-project-structure/01-workspaces/README.md`

## Run

From the repo root:

```bash
cd lessons/02-project-structure/00-ingots
fe check app

cd ../01-workspaces
fe check .
```
