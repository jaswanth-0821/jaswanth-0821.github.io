---
layout: default
permalink: /images/
title: images
description: A collection of visuals from different moments of my work and life
nav: true
nav_order: 4

images:
  - assets/img/1.jpg
  - assets/img/2.jpg
  - assets/img/3.jpg
  - assets/img/5.jpg
  - assets/img/6.jpg
  - assets/img/7.jpg
  - assets/img/8.jpg
  - assets/img/9.jpg
  - assets/img/10.jpg
  - assets/img/11.jpg
  - assets/img/12.jpg
  - assets/img/7.jpg
  - assets/img/8.jpg
---

<div class="masonry-gallery">
  {% for image in page.images %}
    <img src="{{ image | relative_url }}" alt="Image {{ forloop.index }}" />
  {% endfor %}
</div>

<style>
.masonry-gallery {
  column-count: 3;
  column-gap: 16px;
  padding: 20px;
}

.masonry-gallery img {
  width: 100%;
  display: block;
  margin-bottom: 16px;
  border-radius: 8px;
  break-inside: avoid; /* Avoid image being broken across columns */
}
</style>

