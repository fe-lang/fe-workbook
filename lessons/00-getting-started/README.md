# Lesson 00 — Getting started

This lesson is a tiny **workspace** with one member that exists (`counter_test/`) and one member that is intentionally missing (`counter/`).

Your job is to create the missing `counter` ingot using `fe new`, then run the tests.

## Run

From this directory:

```bash
cd lessons/00-getting-started
fe test counter_test
```

You should see an error because the workspace member `counter` is missing.

## Fix

Create the missing member (from the workspace root):

```bash
fe new counter
```

Then re-run the tests:

```bash
fe test counter_test
```

If you want to run the tests that `fe new` generated in the `counter` ingot too:

```bash
fe test counter
```
