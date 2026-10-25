## Rust

### Tips

- Using the ! symbol indicates a macro in Rust. Macros is Rust is the way to extend Rust functionality.

- This file is in the TOML (Tom’s Obvious, Minimal Language) format, which is Cargo’s configuration format.

- In Rust, packages of code are referred to as crates.

### Cargo

- [Cargo Doc](https://doc.rust-lang.org/cargo/)
- [Rust repositories - Creates](https://crates.io/)

Cargo is the package manager in Rust. 
The file that handle the cargo setup is Cargo.toml.

One easy way to get that Cargo.toml file is to run "cargo init", which will create it for you automatically.

[package], is a section heading that indicates that the following statements are configuring a package.

[dependencies], is the start of a section for you to list any of your project’s dependencies

Cargo.lock. This file keeps track of the exact versions of dependencies in your project. You won’t ever need to change this file manually; Cargo manages its contents for you.

#### Create a project

```rust
$ cargo new
```

#### build your project by entering the following command:

```rust
$ cargo build
```

#### Run your project

```rust
$ cargo run
```

#### Check the code

This command check if the code compiles but doesn't produce an executable.
 - cargo check is much faster than cargo build because it skips the step of producing an executable.

```rust
$ cargo check
```

#### Release a project

```rust
$ cargo build --release
```

## Standar library

[Std Doc](https://doc.rust-lang.org/std/prelude/index.html)

## Comments

Use `//` to add a line comment.

```rust
let apples = 5; // This is an inline comment
```

## Variables

By default the variables in Rust are inmutable. To make a variable mutable, we add mut before the variable name:

```rust
let apples = 5; // immutable
let mut bananas = 5; // mutable
```