# Embedded Systems & IoT in Ruby

While not known for running on microcontrollers, Ruby has specialized implementations that make it a viable, high-level language for IoT.

## Implementations

*   **[mruby](https://mruby.org/):** The lightweight implementation of the Ruby language. It can be embedded in C/C++ applications and runs on resource-constrained devices.
*   **[PicoRuby](https://github.com/picoruby/picoruby):** An implementation of mruby specifically for the Raspberry Pi Pico and other RP2040 microcontrollers.
*   **[Artoo](https://artoo.io/) / [Cylon.js](https://cylonjs.com/) (Ruby support):** Frameworks for robotics and physical computing.

## Use Cases

*   **High-Level Logic:** Running business logic on an IoT Gateway (Raspberry Pi) while outsourcing real-time constraints to C/Rust.
*   **Scripting:** allowing end-users to script device behavior in a safe, readable language.

## Gaps

Ruby is not suitable for "hard real-time" constraints. For that, it is best paired with C or Rust (via FFI).
