# Helios - HTTP Server

`helios-http` is an HTTP service layer intended to sit on top of Helios networking primitives. The goal is a high-level proof-of-concept app riding on lower-level stack components.

For top-level build scripts, shared targets, and project-wide setup, use the main Helios README:  
https://github.com/mhambre/helios

## Build / Run / Debug

Direct cargo build:

```bash
cargo +nightly build -p helio-http --target x86_64-unknown-linux-gnu
```

Run directly after build:

```bash
./target/x86_64-unknown-linux-gnu/debug/helio-http
```

If/when this crate is wired into your root build aliases, use:

```bash
just build http release
just build http debug
just gdb http
```
