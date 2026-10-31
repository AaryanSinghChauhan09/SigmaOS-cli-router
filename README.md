# SigmaOS CLI Router

A Rust command-routing model. `CliRouter` registers command metadata, resolves routes against arguments, groups and lists commands, and records route conflicts.

Automatic directory discovery is currently a placeholder: `auto_register_from_dir` verifies the directory exists but registers zero commands. The crate does not itself execute resolved commands; review integration code before relying on it as a dispatcher.

## Build

The manifest references sibling [`SigmaOS-kernel`](../SigmaOS-kernel). From the SigmaOS checkout:

```sh
cargo check --manifest-path SigmaOS-cli-router/Cargo.toml --lib
```

## License

GPL-3.0-or-later. See [`Cargo.toml`](Cargo.toml).
