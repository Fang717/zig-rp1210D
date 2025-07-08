# RP1210D Implementation in Zig

This project is a complete implementation of the [RP1210D](https://www.atabusinesssolutions.com/Shopping/Product/viewproduct/2675472/TMC-Individual-RP), the most recent revision of the **RP1210** communications interface standard, written entirely in the [Zig programming language](https://ziglang.org/).

The purpose of this project is to provide a **native Zig library** for developing diagnostic and reprogramming tools compatible with RP1210-compliant devices such as the **Nexiq USB-Link**, **DrewLinQ**, **Dearborn DPA5**, and others.

## Features

- 🧩 Pure Zig codebase — no C or Windows headers required.
- ⚙️ Implements all RP1210D functions:
  - `RP1210_ClientConnect`
  - `RP1210_ClientDisconnect`
  - `RP1210_SendMessage`
  - `RP1210_ReadMessage`
  - `RP1210_ReadVersion`
  - `RP1210_SendCommand`
  - `RP1210_GetHardwareStatus`
  - `RP1210_GetErrorMsg`
- 🪟 Works with Windows `.dll` interface model.
- 🧪 Designed for robust unit testing and cross-platform support.
- 🔧 Can be used to build Zig-based diagnostic tools, logging systems, or reflashing utilities.

## Why Zig?

Zig offers modern tooling, a simpler build system, and direct memory control, making it ideal for systems programming. Compared to C, it eliminates many of the pitfalls (like undefined behavior) and provides a more ergonomic developer experience.

## Getting Started

### Requirements

- Zig 0.15.0 or later
- Windows (for RP1210 DLLs)
- RP1210-compliant hardware and drivers

### Build

```bash
zig build
