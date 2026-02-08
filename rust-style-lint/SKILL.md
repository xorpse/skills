---
name: rust-style-lint
description: Rust style linting
---

# Rust style

To ensure consistent and readable code ALWAYS ensure the following lint passes are executed as sub-agents:

clippy:

```sh
cargo clippy --no-deps
cargo clippy --fix
```

dylint:

```sh
cargo dylint --git https://github.com/xorpse/rust-style --pattern '*'
```

It is imperative that all issues raised by linters are addressed. Treat each warning as an error and a blocker to complete the task you are working on.

## Troubleshooting

If `cargo dylink` does not run correctly, ensure it is installed:

```sh
cargo install cargo-dylint dylint-link
```
