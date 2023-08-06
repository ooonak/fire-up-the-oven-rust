# fire-up-the-oven-rust
Example Hello World for inclussion in a BitBake meta data layer.

## Setup
```bash
$ cargo init fire-up-the-oven-rust
```

## Build and run
```bash
$ cd fire-up-the-oven-rust
$ cargo build
$ cargo run
```

## Prepare for BitBake
First we have to append to Cargo.toml

```bash
authors = ["Oonak Kanoo <a@b.c>"]
license = "MIT"
description = "Another Hello World"
repository = "https://github.com/ooonak/fire-up-the-oven-cmake.git"
```

The following requires that you have installed the bitbake cargo toolchain.
```bash
$ cargo install cargo-bitbake
```

Then generate the BitBake recipe.

```bash
$ cargo bitbake
No package.homepage set in your Cargo.toml, trying package.repository
Wrote: fire-up-the-oven-rust_0.1.0.bb
```
