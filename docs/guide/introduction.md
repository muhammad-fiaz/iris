---
title: "Introduction to Iris"
description: "Introduction to Iris — a pure-Rust computer vision library with zero C dependencies, GPU acceleration, and multi-threaded CPU support."
keywords: ["introduction", "why iris", "pure rust cv", "zero dependencies", "memory safe", "type safe"]
---

> [!NOTE]
> This project is still in active development. APIs and features may change before the first stable release.

# Introduction

Welcome to **Iris**! This library provides high-performance computer vision algorithms, image manipulation tools, and deep learning model hosting fully in safe Rust.

## Why Iris?

Traditional computer vision libraries are often large C++ codebases. Using them from Rust requires binding wrappers, which introduce:

- Complicated build toolchains, especially on Windows or bare-metal environments.
- Linking conflicts with system-level dynamic libraries.
- Unsafe memory pointers that bypass Rust's borrow checker.

**Iris** takes a different approach — every algorithm is implemented natively in Rust:

- **Memory Safe**: All code runs within Rust's ownership system. No null pointer dereferences, no buffer overflows, no data races.
- **Type Safe**: Strong compile-time type guarantees prevent shape mismatches, invalid tensor operations, and API misuse.
- **Zero-Dependency Compilation**: Clean Cargo builds with no external C/C++ system libraries required.
- **Modern Hardware Acceleration**: Run the same operations on CPU, WGPU (Vulkan, DX12, Metal), or CUDA by switching the backend type parameter.
- **Rayon Multi-Threading**: CPU-intensive loops scale automatically to all available cores.
