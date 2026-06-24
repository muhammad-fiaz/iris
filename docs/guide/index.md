---
title: "What is Iris?"
description: "Iris is a fast, pure-Rust computer vision library framework powered by Burn. Learn about its goals, architecture, and modular design."
keywords: ["Iris", "what is iris", "rust computer vision", "burn framework", "CV library"]
---

# What is Iris?

**Iris** is a fast computer vision library written entirely in pure Rust. It leverages the **Burn** framework for GPU/CPU tensor computations — memory safe, type safe, with no external C/C++ dependencies.

## Key Goals

1. **Pure Rust Ecosystem**: Keep dependencies clean, safe, and fully compiled under the Cargo toolchain.
2. **Familiar CV API**: Provide developers with a clean, modern API covering Image I/O, Filters, Gradients, Contour tracking, Cameras, Drawing, and Detection.
3. **Deep Learning First**: Out-of-the-box loading of ONNX and Safetensors models, powered by Burn backends (WGPU, CUDA, Metal, Ndarray).
4. **Multi-Threaded CPU Acceleration**: All computationally intensive CPU operations are parallelized using Rayon, allowing high throughput when not running on a GPU.

## Project Structure

Iris is designed with modularity in mind:
- **`core`**: Contains the basic matrix representations (`Mat`), geometric types (`Point`, `Rect`, `Size`, `Scalar`), and randomized number generators.
- **`image`**: Provides representation, file I/O, resizing, remapping, and geometric warping.
- **`filters`**: Includes box blur, Gaussian blur, median filter, bilateral filter, and separable 2D filtering.
- **`edges`**: Offers Canny edge detection, Sobel, Scharr, and Laplacian gradients.
- **`dnn`**: Handles neural network weight loading (Safetensors, Bin, ONNX) and model prediction.
- **`gui`**: A modern windowing manager that supports trackbars, buttons, and custom layout render loops.
