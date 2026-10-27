---
layout: post
title: "hip-tile — kernel GPU in stile cuTile, in Rust"
permalink: /it/projects/hip-tile/
alt: /projects/hip-tile/
excerpt: "Kernel a tile in stile cuTile per GPU AMD, scritti in puro Rust e compilati direttamente in codice macchina AMDGPU."
---

<figure class="project-detail-figure">
  <img src="/assets/hip_tile_legogears.png" alt="Detection LegoGears calcolate su una iGPU Radeon 680M">
  <figcaption>YOLOv4-tiny su LegoGears con una iGPU Radeon 680M: 4,8 ms per frame, 92× più veloce del riferimento su CPU.</figcaption>
</figure>

## Panoramica

hip-tile porta il modello di programmazione cuTile sulle GPU AMD. Un kernel si scrive come operazioni su tile intere (`load_tile`, `mma`, `map`, `store_tile`). `rustc` lo compila direttamente in codice macchina AMDGPU, e `cargo` lo costruisce, lo incorpora e lo lancia tramite HIP. Niente C++, niente `hipcc`, niente assembly inline.

## Cosa include

- **Puro Rust dal kernel al lancio:** codice device `#![no_std]` compilato per `amdgcn-amd-amdhsa`, binding HIP scritti a mano lato host.
- **Lanci tipizzati:** `#[kernel]` genera il punto di ingresso GPU e un launcher host tipizzato, quindi argomenti sbagliati sono errori di compilazione.
- **hip_darknet:** un port in Rust di un detector Darknet YOLOv4-tiny che gira, e si addestra, su GPU con i kernel hip-tile.

## Risultati

Misurati su iGPU Radeon 680M (gfx1031, 12 CU, RDNA2), f32:

- La GEMM a tile raggiunge 2,28 TFLOP/s con N = 2048, 1,19× rocBLAS.
- Forward di YOLOv4-tiny: 4,8 ms per frame su GPU contro 443 ms su un thread CPU.
- Un passo di training completo (forward, loss, backward, SGD) richiede circa 0,3 s con batch 16.
- Le detection GPU e CPU coincidono su 10 immagini, con recall e precision pari a 1,0 rispetto alle etichette del dataset.

Codice: [github.com/iltranqui/hip_tile](https://github.com/iltranqui/hip_tile)
