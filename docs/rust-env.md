# Setup Rust

### 1. Install `Rust`:

```shell
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

- This command will download and install the Rust toolchain:
 
  - The `Rust` compiler (rustc)
  - The `Cargo` package manager (cargo)
  - The `rustup` tool for managing the Rust toolchain and versions


### 2. Add `Rust` to your path:

```shell
source $HOME/.cargo/env
```

### 3. Check installation:

```shell
rustc --version
cargo --version
```

### 4. Install useful tools: 
  

```shell
sudo apt install build-essential pkg-config libssl-dev -y
```

This is necessary to compile many crates, especially those dealing with cryptography or `HTTP`


```shell
cargo install cargo-edit cargo-watch
```

- `cargo-edit`: Makes it easier to add/remove dependencies (`cargo add <crate>`)
- `cargo-watch`: Allows you to run code automatically when detecting changes (`cargo watch -x run`)

- In VSCode, install the [Rust Analyzer](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer) extension for debugging.

### 5. Create a new project:


```shell
cargo new <project_name>
cd <project_name>
cargo run
```
