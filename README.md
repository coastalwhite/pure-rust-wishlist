# Pure Rust Wishlist

This is a list of pure rust crates that I, personally, would love to see and
some explaination of why I would want them. I don't think I will take the time
to work on any of them so feel free to start them yourself. Mostly, this list
allows me some peace of mind knowing that I do not have to work on an idea
myself.

If you make or find any project that are on this list to exist let me know.

This idea is very similar to the [Not-Yet-Awesome Rust] list.

[Not-Yet-Awesome Rust]: https://github.com/not-yet-awesome-rust/not-yet-awesome-rust

## General Tooling

### Plymouth

### WiFi selector

### UDev Replacement

### LibUSB

## Embedded

### RISC-V Linker

### Dynamic-Translation Emulation

Similar to [QEMU].

Advantages:
- Programmatic Access / Static Linking
- `#[platform-test]` macro, which allow specific tests to happen on specific
  platforms
- Speed, memory footprint
- WASM

## Hardware Design

### Logic Minimization
### RTL Simulator
### TCL Interpreter

## Electrical Engineering

### SPICE

Make a mostly [SPICE] compatible tool for electronic circuit simulation. Since
there are so many variants of SPICE (LTSpice, HSpice, etc.), it is not possible
to make it fully compatible.

Advantages:
- Programmatic Access / Static Linking
- WASM

## Security

### Pluggable Authentication Modules

It would be really nice to rewrite [PAM] in Rust. It would allow for static
linking and greater security. It might also be nice to just change up the
authentication model entirely, but I am guessing no-one will ever go for that.
In general, PAM is a complete stability mess.

Advantages:
- Programmatic Access / Static Linking
- Security

## Visualization and UI

### Eclipse Layout Kernel

The _Eclipse Layout Kernel_ ([ELK]) could make many diagram and visualization
tools easier.

Advantages:
- Programmatic Access / Static Linking
- Speed, memory footprint
- WASM

### FontConfig

Imagine being able to static link [FontConfig] and being
able to guarentee that it exists. Problem being that each distribution applies
it's own patches for it.

### Text Rendering

### Code annotation tool

Imagine like a mix between [WaveDrom] and [Carbon]. Being able to declaratively
generate figures for slides and tweets.

[QEMU]: https://www.qemu.org/
[SPICE]: https://en.wikipedia.org/wiki/SPICE
[PAM]: https://en.wikipedia.org/wiki/Pluggable_authentication_module
[ELK]: https://eclipse.dev/elk/
[FontConfig]: https://www.freedesktop.org/wiki/Software/fontconfig/
[wavedrom]: https://wavedrom.com/
[Carbon]: https://carbon.now.sh/