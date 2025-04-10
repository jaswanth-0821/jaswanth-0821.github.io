---
layout: default
permalink: /images/
title: images
description: A collection of visuals from different moments of my work and life
nav: true
nav_order: 4

images:
  # - assets/img/my_images/_93A2095.jpg
  - assets/img/my_images/IMG_0053.jpg
  - assets/img/my_images/IMG_20220101_162437-01.jpeg
  - assets/img/my_images/IMG_20240511_191351.jpg
  - assets/img/my_images/IMG-20240721-WA0010.jpg
  - assets/img/my_images/IMG20220101161717-01.jpeg
  - assets/img/my_images/PJ_hand.png.jpg
  - assets/img/my_images/SHI01681.JPG
  - assets/img/my_images/SHI01146.JPG
  - assets/img/my_images/IMG_9957.jpg
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

