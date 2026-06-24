---
layout: home

hero:
  name: Iris
  text: Native Rust Computer Vision
  tagline: A fast computer vision library in pure Rust.
  image:
    src: /logo.svg
    alt: Iris Logo
  actions:
    - theme: brand
      text: Get Started
      link: /guide/getting-started
    - theme: alt
      text: View on GitHub
      link: https://github.com/muhammad-fiaz/iris

banner:
  content: "Note: This project is still in active development. APIs and features may change before the first stable release."
  type: warning

features:
  - icon: 🦀
    title: Pure idiomatic Rust
    details: Written natively in Rust from the ground up. Zero unsafe wrappers, zero external C/C++ dependencies.
  - icon: 🔥
    title: Burn Deep Learning
    details: Fully integrated with the Burn framework. Load ONNX, Safetensors, or native Burn model weights out of the box.
  - icon: ⚡
    title: GPU & WGPU Accelerated
    details: Harness hardware acceleration across WGPU, CUDA, Metal, and Vulkan automatically using compile-time features.
  - icon: 🧵
    title: Multi-Threaded CPU
    details: Automatic multi-threaded parallel execution across image filters, geometry warps, morphology, and drawing using Rayon.
  - icon: 🖥️
    title: Cross-Platform Direct UI
    details: Easy GUI window creation, mouse callbacks, trackbars, and rendering backends supported by Zed's GPUI framework.
  - icon: 🎯
    title: Type-Safe & Memory-Safe
    details: Built entirely in safe Rust — no unsafe code, no FFI bindings, no null pointers. Guaranteed memory safety and type safety at compile time.
---
