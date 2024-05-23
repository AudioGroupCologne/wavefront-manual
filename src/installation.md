# Installation

## Pre-compiled binaries

<!-- this is more or less (more more) stolen from the mdbook book -->
Executable binaries are available for download on the [GitHub Releases page](https://github.com/nichilum/wavefront/releases). Download the binary for your platform (Windows, macOS, or Linux) and extract the archive. The archive contains the wavefront executable.

## Build from source using Rust
To build the wavefront executable from source, you will first need to install Rust and Cargo. Follow the instructions on the [Rust installation page](https://www.rust-lang.org/tools/install). Wavefront is build using Rust version 1.78.

<!-- I don't know which Rust versions we can officially support -->

Once Rust is installed, clone and enter the Github repository:

```bash
git clone https://github.com/nichilum/wavefront.git
cd wavefront
```

Build wavefront in release mode using:

```bash
cargo run --release
```
