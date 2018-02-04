# Hello World

## RustのInstall
```
$ curl https://sh.rustup.rs -sSf | sh
% rustup --help                                                                                                                         

rustup 1.10.0 (c6a8f7c60 2018-01-25)
The Rust toolchain installer

USAGE:
    rustup [FLAGS] <SUBCOMMAND>

FLAGS:
    -v, --verbose    Enable verbose output
    -h, --help       Prints help information
    -V, --version    Prints version information

SUBCOMMANDS:
    show           Show the active and installed toolchains
    update         Update Rust toolchains and rustup
    default        Set the default toolchain
    toolchain      Modify or query the installed toolchains
    target         Modify a toolchain's supported targets
    component      Modify a toolchain's installed components
    override       Modify directory toolchain overrides
    run            Run a command with an environment configured for a given toolchain
    which          Display which binary will be run for a given command
    doc            Open the documentation for the current toolchain
    man            View the man page for a given command
    self           Modify the rustup installation
    set            Alter rustup settings
    completions    Generate completion scripts for your shell
    help           Prints this message or the help of the given subcommand(s)

DISCUSSION:
    rustup installs The Rust Programming Language from the official
    release channels, enabling you to easily switch between stable,
    beta, and nightly compilers and keep them updated. It makes
    cross-compiling simpler with binary builds of the standard library
    for common platforms.

    If you are new to Rust consider running `rustup doc --book` to
    learn Rust.
```

## Cargoのversion確認

CargoはRustのビルドシステムであり、パッケージマネージャー。
また、コードのビルド、依存するライブラリのDownload、ライブラリのビルドも作る。

```
$ cargo --version
cargo 0.24.0 (45043115c 2017-12-05)
```

## ビルド

```
$ cargo build
   Compiling hello_world v0.0.1 (file:///home/yourname/projects/hello_world)
$ ./target/debug/hello_world
Hello, world!
```

```
$ cargo run
     Running `target/debug/hello_world`
Hello, world!
```
