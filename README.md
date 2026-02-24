# Fe Workbook

A small workbook for learning the Fe language via intentionally broken exercises.

All exercises live under `lessons/`.

## Prerequisites

- The `fe` CLI
  - Install: `$ curl -fsSL https://raw.githubusercontent.com/argotorg/fe/master/feup/feup.sh | bash` 
- Optional: `solc` if you want to use the Yul backend (`--backend yul`)
- An editor with Fe syntax/LSP support (you can run `fe lsp`)
  - [zed](https://github.com/fe-lang/zed-fe)
  - [emacs](https://github.com/fe-lang/emacs-fe)
  - [neovim](https://github.com/fe-lang/nvim-fe)
  - [vscode](https://github.com/fe-lang/vscode-fe)

## How to use this repo

- Each lesson has a `README.md` with run instructions.
- Exercises are meant to be fixed. Follow the `PROBLEM:` / `EXERCISE:` markers and compiler errors until things compile and tests pass.

## Start here

- Lesson 00 — Getting Started: `lessons/00-getting-started/README.md`
- Lesson 01 — Language Basics: `lessons/01-language/README.md`
- Lesson 02 — Project Structure: `lessons/02-project-structure/README.md`
