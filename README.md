# RustyGecko seed project.

This is an example project for starting new projects on the RustyGecko platform.
The example shows how to blink a led on the Giant Gecko Starter Kit (STK3700). 

## Prerequisites

To run this project your system contain
- [Nightly Rust compiler](http://www.rust-lang.org/install.html)
- [arm-none-eabi-gcc](https://launchpad.net/gcc-arm-embedded/+download)

## Building

Run the following commands to produce a `seed.bin` file
```
cargo build --target thumbv7m-none-eabi
arm-none-eabi-objcopy -O binary target/thumbv7m-none-eabi/debug/seed seed.bin
```

The `seed.bin` file can now be flashed to the Starter Kit
