# Rust to WASM sample

This repository contains a simple Rust library which exposes the `multiply` function. You can build the library for `wasm32-wasi` using `cargo build --target wasm32-wasi`

## Invoke the multiply function

You can invoke the `multiply` function `wasmtime`:

```bash
# run WASM module via wasmtime
wasmtime --invoke multiply ./target/wasm32-wasi/debug/sample.wasm 3 3 4
# will print 36
```
