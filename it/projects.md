---
layout: page
title: Progetti
permalink: /it/projects/
alt: /projects/
---

<p class="writing-page-intro">Esperimenti di computer vision e progetti selezionati.</p>

<div class="work-grid project-archive">
  <article class="work-card">
    <img class="project-card-image" src="/assets/Kaggle_book.jpg" alt="Il libro The Kaggle Book annotato con un cuboide 3D e con etichette 2D degli oggetti" loading="lazy">
    <p class="card-kicker">COMPUTER VISION 3D · ESPERIMENTO SU DATASET</p>
    <h3><a href="/it/projects/kaggle-book-3d-detection/">Kaggle Book — Detection 3D</a></h3>
    <p>Un esperimento di computer vision che usa un libro come oggetto reale per la detection di cuboidi 3D. L’immagine mostra gli otto vertici del cuboide e le etichette 2D dell’oggetto annotate attorno al libro.</p>
    <ul class="tag-list"><li>Detection 3D</li><li>Keypoint del cuboide</li><li>Etichette 2D</li></ul>
  </article>
  <article class="work-card">
    <img class="project-card-image" src="/assets/hip_tile_legogears.png" alt="Detection LegoGears calcolate su una iGPU Radeon 680M" loading="lazy">
    <p class="card-kicker">PROGRAMMAZIONE GPU · RUST · AMD</p>
    <h3><a href="/it/projects/hip-tile/">hip-tile — kernel GPU in stile cuTile, in Rust</a></h3>
    <p>Kernel GPU a tile per AMD, scritti in puro Rust e compilati da <code>rustc</code> direttamente in codice AMDGPU. Un detector YOLOv4-tiny, addestrato ed eseguito su GPU, lo dimostra su un modello reale.</p>
    <ul class="tag-list"><li>Rust</li><li>HIP</li><li>AMDGPU</li><li>YOLOv4-tiny</li></ul>
  </article>
</div>
