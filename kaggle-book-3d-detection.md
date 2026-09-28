---
layout: post
title: "Kaggle Book — 3D Detection"
permalink: /projects/kaggle-book-3d-detection/
excerpt: "A computer-vision experiment annotating a real-world book with 3D cuboid keypoints and 2D boxes."
---

<figure class="project-detail-figure">
  <img src="/assets/Kaggle_book.jpg" alt="A book annotated with a projected 3D cuboid and 2D object labels">
  <figcaption>The book is labeled with its projected cuboid corners and 2D annotations.</figcaption>
</figure>

## Overview

This project explores 3D object detection using a physical copy of *The Kaggle Book*. The image shows the book annotated as a 3D cuboid: its projected corners are labeled so the object's shape and orientation can be represented in a single image.

## Annotations

The example combines two kinds of labels:

- **3D cuboid:** eight projected corner points describe the book's visible 3D shape.
- **2D boxes:** additional object labels mark regions in the image alongside the cuboid annotation.

The goal is to work with both 2D detections and 3D cuboid annotations in a computer-vision dataset.
