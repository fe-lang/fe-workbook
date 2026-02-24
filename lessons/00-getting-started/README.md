# Lesson 00 — Getting Started

This lesson is a single, standalone Fe contract: `cool_coin.fe` (an ERC‑20 token called “CoolCoin”).

## Goal

- Make sure the `fe` CLI works on your machine
- Learn the basic workflow: `check` →  `test` →  `build`
- See what a test looks like

## Run

From the repo root:

```bash
cd lessons/00-getting-started

# Typecheck + diagnostics (fast)
fe check cool_coin.fe

# Compile to bytecode (writes artifacts to `out/` by default)
fe build cool_coin.fe

# Run the ERC20 test suite (tests live at the bottom of `cool_coin.fe`)
fe test cool_coin.fe
```

## What’s in the contract?

`CoolCoin` implements the ERC‑20 interface:

- `name`, `symbol`, `decimals`
- `totalSupply`, `balanceOf`, `allowance`
- `transfer`, `approve`, `transferFrom`
- plus a simple `mint(address,uint256)` extension (used by the tests)

