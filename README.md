# 🍭 Candy's Golden IRs

This repository contains the generated IRs for the [`packages/Examples/` directory](https://github.com/candy-lang/candy/tree/main/packages/Examples) of the [Candy repository](https://github.com/candy-lang/candy).

IRs, or Intermediate Representations, are the outputs of different stages of the Candy compiler.
For more information about our Compiler architecture, please refer to the following file: https://github.com/candy-lang/candy/blob/main/compiler/frontend/src/README.md.

Each branch name in this repository is named after the commit hash of the Candy repository that generated the IRs.
(Plus a trailing underscore since Github doesn't allow branch names that have the same format as commit hashes.)

## Why?

We want to make sure that the compiler output doesn't change unexpectedly.
Therefore, our CI pipeline generates the IRs for each commit in the Candy repository and compares them to the previous IRs in this repository.
Changes can show:

- the changes a new optimization is performing,
- changes to files in the example directory, or
- a bug that was introduced in the compiler.
