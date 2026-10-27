---
layout: post
title: "Kaggle Book — Detection 3D"
permalink: /it/projects/kaggle-book-3d-detection/
alt: /projects/kaggle-book-3d-detection/
excerpt: "Un esperimento di computer vision che annota un libro reale con keypoint di cuboidi 3D e box 2D."
---

<figure class="project-detail-figure">
  <img src="/assets/Kaggle_book.jpg" alt="Un libro annotato con un cuboide 3D proiettato e con etichette 2D degli oggetti">
  <figcaption>Il libro è etichettato con i vertici proiettati del cuboide e con annotazioni 2D.</figcaption>
</figure>

## Panoramica

Questo progetto esplora la detection di oggetti 3D usando una copia fisica di *The Kaggle Book*. L’immagine mostra il libro annotato come cuboide 3D: i suoi vertici proiettati sono etichettati, così forma e orientamento dell’oggetto possono essere rappresentati in una sola immagine.

## Annotazioni

L’esempio combina due tipi di etichette:

- **Cuboide 3D:** otto punti proiettati dei vertici descrivono la forma 3D visibile del libro.
- **Box 2D:** altre etichette dell’oggetto segnano regioni dell’immagine accanto all’annotazione del cuboide.

L’obiettivo è lavorare sia con detection 2D sia con annotazioni di cuboidi 3D in un dataset di computer vision.
