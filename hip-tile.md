---
layout: post
title: "hip-tile — cuTile-style GPU kernels in Rust"
permalink: /projects/hip-tile/
alt: /it/projects/hip-tile/
excerpt: "cuTile-style tile kernels for AMD GPUs, written in pure Rust and compiled straight to AMDGPU machine code."
---

<figure class="project-detail-figure">
  <img src="/assets/hip_tile_legogears.png" alt="LegoGears detections computed on a Radeon 680M iGPU">
  <figcaption>LegoGears YOLOv4-tiny on a Radeon 680M iGPU: 4.8 ms per frame, 92× faster than the CPU reference.</figcaption>
</figure>

## Overview

hip-tile brings the cuTile programming model to AMD GPUs. A kernel is written as operations on whole tiles (`load_tile`, `mma`, `map`, `store_tile`). `rustc` compiles it straight to AMDGPU machine code, and `cargo` builds, embeds and launches it through HIP. There is no C++, no `hipcc` and no inline assembly.

## What it includes

- **Pure Rust from kernel to launch:** `#![no_std]` device code built for `amdgcn-amd-amdhsa`, hand-written HIP bindings on the host.
- **Typed launches:** `#[kernel]` generates the GPU entry point and a typed host launcher, so mismatched arguments are compile errors.
- **hip_darknet:** a Rust port of a Darknet YOLOv4-tiny detector that runs, and trains, on the GPU using hip-tile kernels.

## Results

Measured on a Radeon 680M iGPU (gfx1031, 12 CUs, RDNA2), f32:

- Tile GEMM reaches 2.28 TFLOP/s at N = 2048, 1.19× rocBLAS.
- YOLOv4-tiny forward pass: 4.8 ms per frame on the GPU against 443 ms on one CPU thread.
- A full training step (forward, loss, backward, SGD) takes about 0.3 s at batch 16.
- GPU and CPU detections match on 10 images, with recall and precision of 1.0 against the dataset labels.

Source: [github.com/iltranqui/hip_tile](https://github.com/iltranqui/hip_tile)
